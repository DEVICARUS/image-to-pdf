<h1 align="center">Welcome to img-to-pdf 👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000" />
</p>

> Creates a PDF file out of images

## Instalation
```sh
npm install img-to-pdf
# OR
yarn add img-to-pdf
```

## Example
```js
const fs = require('fs');
const imgToPDF = require('./main');

const pages = [
   "pages/1.png",
   "pages/2.png",
   "pages/3.png"
]

imgToPDF(pages, 'A4')
   .pipe(fs.createWriteStream('output.pdf'));

```

A list of all accepted page sizes can be found [here](sizes.json).
