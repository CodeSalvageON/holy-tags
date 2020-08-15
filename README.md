# holy-tags
Holy Tags that make your website a little more secure.

![Holy Tags Logo](https://holy-tags.codesalvageon.repl.co/src/images/holytags.PNG)

## Where can I use Holy Tags?
1. You can use Holy Tags in cases where you don't want to install a security plugin on your website.
2. You want to get rid of specific cross site scripting attacks(XSS).
3. You're too lazy to write your own XSS protection script.

## Features
 - Link (Anchor Tag) blocking
 - Attribute blocking (Blocks all attributes in a tag)
 - Tag blocking (Removes all tags inside of the <crucifix> element, but is ineffective against <script> tags)
 - Removes HTML elements from the first form value automatically when forms are submitted
 - HTML Removal Function

## What Holy Tags can't do
 - Automatically remove HTML elements from the first form value from multiple forms
 - Block <script> tags using the <crucifix> tag

## How to use Holy Tags
Put this in your `<head>` tag somewhere...

```
<link href="https://holy-tags.codesalvageon.repl.co/src/css/holy.min.css" rel="stylesheet">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script src="https://holy-tags.codesalvageon.repl.co/src/scripts/script.min.js"></script>
```

### Holy tags and where to use them
`<rosary>`- Removes all links (anchor tags) inside the rosary tag.
<br>
`<rosary><a href="">This link will be removed, turning it into plain text.</a></rosary>`
<br>
`<confession>`- Removes all attributes of the elements inside the confession tag.
<br>
```
<confession><p style="color: blue">This paragraph tag was supposed to be blue, but the confession tag has removed the style attribute.</p></confession>
```
