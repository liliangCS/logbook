## 对文件进行 `gzip` 压缩

```javascript
const fs = require("node:fs")
const zlib = require("node:zlib")

function compFile(entryPath, outputPath) {
  const gzip = zlib.createGzip()
  fs.createReadStream(entryPath)
    .pipe(gzip)
    .pipe(fs.createWriteStream(outputPath))
}

compFile("./data.txt", "./data.gz")
```
