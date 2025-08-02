# webfs.js

Node.js `fs` API in browser on top of OPFS (Origin Private File System).

This TypeScript library provides a familiar Node.js filesystem interface for browser environments using the Origin Private File System API.

## Usage

Simply load `webfs.js` in your browser environment:

```html
<script src="https://cdn.jsdelivr.net/npm/webfs.js/dist/index.js"></script>
```

and then you will have access to the `fs` object that mimics Node.js `fs` API:

```javascript
const fs = window.fs;
fs.writeFile('/path/to/file.txt', 'Hello, World!')
  .then(() => {
    console.log('File written successfully');
  })
  .catch((err) => {
    console.error('Error writing file:', err);
  });
```

[See live demo](https://jsfiddle.net/mos4ua9d/2/).
