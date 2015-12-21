# Markdown to Html

Parse markdown to html. Support for Markdown-extra(tables, definition lists, fenced code blocks, footnotes, table of contents), Latex, UML diagrams.

## How to use it
```javascript
<script src="markdown-to-html.min.js"></script>
<script>
var markdown = `# h1
# h2
# h3
`;
// 1. Parse markdown to id="content" dom
markdownToHtml(markdown, document.getElementById('content'));

// 2. Parse markdown to id="content" dom and get the html by callback
markdownToHtml(markdown, document.getElementById('content'), function(html) {
	console.log(html);
});

// 3. Just get the html
markdownToHtml('# h1', function(html) {
  console.log(html);
});

</script>
```

## Thanks to

* PageDown, the Markdown library used by Stack Overflow
* https://github.com/jmcmanus/pagedown-extra
* http://bramp.github.io/js-sequence-diagrams
* http://adrai.github.io/flowchart.js
* http://www.mathjax.org
* https://stackedit.io

## LICENSE

LEANOTE - NOT JUST A NOTEPAD!

Copyright 2015 by the contributors.

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

Leanote Markdown to Html is licensed under the GPL v2.

[LICENSE](https://github.com/leanote/markdown-to-html/blob/master/LICENSE)
