# Markdown-It Wiki Custom Links


Renders Wiki-like links in [markdown-it](https://github.com/markdown-it/markdown-it). This is useful for making Markdown-based wikis.

## Usage

Install this into your project:

```bash
npm --save install markdown-it-wikicustom
```

...and *use* it:

```js
const wikilinks = require('markdown-it-wikilinks')(options)
const md = require('markdown-it')()
    .use(wikilinks)
    .render('Click [[Wiki Links|here]] to learn about [[/Wiki]] links.')
```

**Output:**

```html
<p>Click <a href="Wiki-Links">here</a> to learn about <a href="Wiki">Wiki</a> links.</p>
```