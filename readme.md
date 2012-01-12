### readme.md test file ###

## Paragraphs
This is a regular paragraph.
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas eget dolor velit, vitae rhoncus nisl. Pellentesque molestie velit eget nunc tempus nec interdum ante commodo. Pellentesque laoreet semper mauris id fermentum. Maecenas vitae libero turpis, sed rutrum velit. Maecenas id augue arcu. Aliquam rhoncus iaculis nulla id pellentesque. Phasellus id libero non est tincidunt tempor sit amet eget neque. Pellentesque eu odio non augue ornare pharetra. Nunc id dui non odio convallis lobortis sit amet nec lectus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Ut euismod varius metus et iaculis. In hac habitasse platea dictumst. Nulla facilisi. Vestibulum ac aliquam risus. Pellentesque vel accumsan risus. Nullam sagittis ultricies ullamcorper.

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.

---
***

> first level quote
>    > nested blockquote
   >    > nested blockquote
> back to first level

---
***

> ### header
> 
> 1. This is the first list item.
> 2. This is the second list item.
> 
> Here's some example code:
> 
> return shell_exec("echo $input | $markdown_script");


* *Italic text*
* _italic_
* **bold**
* __bold__

\* escaped asteriks \*

======================================================
------------------------------------------------------

## Heads

# h1 title
## h2 title
### h3 title
#### h4 title
##### h5 title
###### h6 title

## table

<table>
    <tr>
        <td>table data</td><td>table data 2</td>
    </tr>
	<tr>
		<td>table data</td>
	</tr>
</table>

#### links
1. [Pluxbox][http://www.pluxbox.nl/]
2. http://daringfireball.net/projects/markdown/syntax

3. This is [an example](http://example.com/ "Title") inline link.

4. [This link](http://example.net/) has no title attribute.
5. See my [About](/about/) page for details.
6. This is [an example][id] reference-style link.
7. This is [an example] [id] reference-style link.
8. [id]: http://example.com/  "Optional Title Here"
9. [link text][a]
10. [link text][A]
11. [Google][]
12. [Google]: http://google.com/

I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"

13. <http://example.com/>
14. <info@pluxbox.nl>

#### copyright
&copy;

#### lists

Unordered list:

* item 1
* item 2
* item 3

+ item 1
+ item 2
+ item 3

- item 1
- item 2
- item 3

Ordered list

1. item 1
2. item 2
3. item 3

1986. What a great season.
1986\. What a great season.


<ol>
	<li>Bird</li>
	<li>McHale</li>
	<li>Parish</li>
</ol>

#### images

![Pluxbox Logo](http://pluxbox.nl/pluxbox/images/logo-pluxbox.png "Pluxbox Logo")

#### Code Blocks
This is a normal paragraph:

    This is a code block.

requires 4 spaces or a tab

    code block start
        code block tab 1 start
            code block tab 2
        code block tab 1 end
    code block end


###### regular code block
`
if(isset($test)) {
    echo $test;
}
`

`` 
`foo`
``

```
if(isset($test)) {
	echo $test;
}
```

###### php code block
```php
<?php
if(isset($test)) {
	echo $test;
}
?>
```

###### html code block
```html
<!DOCTYPE html>
<html>
    <head>
        <title>test</title>
    </head>
<body>
    <h1>test</h1>
</body>
</html>
```

###### javascript code block
```javascript
<script type="text/javascript"> 
	var player = new PB.Player(
        [{
            title: 'title',
            url: 'url',
            codec: 'mp3',
            stream: true
        },
</script>
```

###### horizontal lines

* * *
***
******
- - -
--------------------------

### Bug tracker ###

Found a bug? Let us know and create an issue on GitHub!

https://github.com/Pluxbox/pbPlayer/issues

*Author(s)*: Pluxbox

- http://www.pluxbox.com/
- https://twitter.com/pluxbox
- https://www.facebook.com/pages/Pluxbox/168484729879371

- [Pluxbox](http://pluxbox.com/ "Pluxbox website")
- [Follow on Twitter](https://twitter.com/pluxbox/ "Follow Pluxbox on Twitter")
- [Facebook page](https://www.facebook.com/pages/Pluxbox/168484729879371 "Pluxbox Facebook page")

*License*

---

\\   backslash
\`   backtick
\*   asterisk
\_   underscore
\{}  curly braces
\[]  square brackets
\()  parentheses
\#   hash mark
\+   plus sign
\-   minus sign (hyphen)
\.   dot
\!   exclamation mark
