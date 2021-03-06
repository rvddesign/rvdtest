![Pluxbox Logo](http://pluxbox.nl/pluxbox/images/logo-pluxbox-black.png "Pluxbox Logo")
# pbPlayer Documentation
## Implementation Guide

pbPlayer is a free and open source mediaplayer developed by Pluxbox written in JavaScript. The pbPlayer works crossbrowser for and supports streams and multiple file playing.

![Radioplayer](http://pluxbox.nl/pluxbox/images/pbplayer/radioplayer.png "Radioplayer")

The pbPlayer has been designed so it can be rendered on a wide range of internet enabled devices. Thanks to the crossbrowser functionality of [pbjs](https://github.com/Saartje87/pbjs "pbjs"), creating a crossbrowser & crossplatform compatible mediaplayer was the next logical step.

### HTML5 player with Adobe Flex (Flash) and Browser Plugin fallback

The pbPlayer has been designed from the core to be a HTML5 native player, which automatically checks if a device actually supports HTML5. If this is not the case, it will fall back to Adobe Flex (Flash). When Adobe Flex is not available, it will fall back to a platform specific plugin. This fallback system guarantees the digital content can be easily delivered to a wide range of products.

- IE6+
- Firefox 3.5+
- Opera 9+
- Google Chrome
- Apple Safari
- IOS browsers (iPad, iPhone and iPod Touch)
- Browsers on Andrioid-phones and tablets

![pbPlayer with Christmas skin](http://pluxbox.nl/pluxbox/images/pbplayer/radio4-kerst.png "pbPlayer Christmas skin")

===

## Structure
*File structure*

```
/pbplayer3/
- flex/
    pbplayer.swf
    pbstreamplayer.swf
- skin/
    - images/
        pbplayer-sprite.png
    skin.css
    skin.js
demo.html
pbjs.js
pbplayer3.js
```
===
## Implementation

### JavaScript

Include the JavaScript files for the pbPlayer in the head  of your page.

- [pbjs.js](https://github.com/Saartje87/pbjs "pbjs")
- pbplayer3.js
- skin.js

Styles are included through JavaScript.

### Single file

pbPlayer can play one or more files. More files can be added through creating an array. When multiple files are added a playlist will appear.

```javascript
var player = new PB.Player({

        title: 'Streaming',
        url: 'http://streamingsite/stream.mp3',
        codec: 'mp3',    // Default mp3
        stream: true    // Default false
    }

    // Specific instance params

    ,{

        renderTo: 'pbplayer',      // id or element node for rendering  e.g. document.getElementById('pbplayer')
        autostart: true,
        volume: 80                 // Options can be overwritten per instance.

    }
);
```

### Playlist variant

```javascript
var player = new PB.Player(

    // Create a playlist by specifing an array.
    // If one song is given, a playlist will not be displayed. 

    [{

        title: 'Streaming',
        url: 'http://streamingsite/stream.mp3',
        codec: 'mp3',   // Default mp3
        stream: true    // Default false

    }, {

        title: 'fragment title',
        url: 'http://radiobox.omroep.nl/fragment/read_sitestat_fragment/33513/33513.mp3',
        codec: 'mp3'

    }]

    // Specific instance params
    ,{

        renderTo: 'pbplayer',      // id or element node for rendering  e.g. document.getElementById('pbplayer')
        autostart: true,
        volume: 80                 // Options can be overwritten per instance.

    }
);
```

### Rendering
pbPlayer is rendered to an HTML element. In the following example we created a div with the id "pbplayer".

```html
<div id="pbplayer"></div>
```
It's not required to be called 'pbplayer' as long as it matches with the **renderTo** decleration.

### Stream
If the file that is played is not a stream, the line **stream:true** can be left out or set to *false*.

### Default options
There's a few default options which can be set for all pbPlayer instances.

```javascript
<script type="text/javascript"> 

// Default options for all pbplayer instances.

PB.Player.options({ 
	 
    skin: 'skin',           // Skin name
    skinPath: 'skin/',      // Path to skin file
    path: 'flex/',          // Current path to swf file 
    volume: 80              // Default volume, min 0 / max 100

});
</script>
```

===
## Bug tracker
Found a bug? Let us know and [create an issue](https://github.com/Pluxbox/pbPlayer/issues "create issue now") on GitHub!

**Author**: [Pluxbox](https://github.com/Pluxbox "Follow Pluxbox on Github")

- [Follow on Twitter](https://twitter.com/pluxbox/ "Follow Pluxbox on Twitter")
- [Facebook page](https://www.facebook.com/pages/Pluxbox/168484729879371 "Pluxbox Facebook page")

&copy; *[Pluxbox](http://pluxbox.com/ "Pluxbox website")*

