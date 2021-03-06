# Sphinx-Documentation
### install
- step 1
<code> npm install -g jsdoc</code>
- Step 2
<code>pip install sphinx-js</code>


### Reference:
- [Jsdoc](https://jsdoc.app/about-tutorials.html)
- [sphinx Officlial Documentation](https://pypi.org/project/sphinx-js/)
- [Sphinx github](https://github.com/mozilla/sphinx-js)
- [Parameter with Properties](https://jsdoc.app/tags-param.html#parameters-with-properties)


### File structure
<ul>
<li>JSDoc
<ul>
<li>custom-template</li>
<li>jsdoc.json</li>
<li>package.json</li>
  <li>src</li>
</ul>
</li>


### jdoc.json
<code> npm i -D jsdoc</code>
~~~~
{
  "source": {
    "include": ["src"],
    "includePattern": ".js$",
    "excludePattern": "(node_modules/|docs)"
  },
  "plugins": ["plugins/markdown"],
  "templates": {
    "cleverLinks": true,
    "monospaceLinks": true
  },
  "opts": {
    "recurse": true,
    "destination": "./docs/",
    "template": "./custom-template",
    "tutorials": "./tutorials",
    "readme": "./readme/readme.md"
  }
}
~~~~
### package.json
~~~~
{
  "name": "jsdoc_example",

  "main": "index.js",
  "scripts": {
    "doc": "jsdoc -c jsdoc.json"
  },
  "devDependencies": {
    "jsdoc": "^3.6.3"
  }
}

~~~~
  <code>npm run doc</code>
  - [Video](https://www.youtube.com/watch?v=YK-GurROGIg)
