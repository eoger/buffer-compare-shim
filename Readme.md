# buffer-compare-shim

Shims Node v0.10.x with v0.12.x `Buffer.compare` and `Buffer.prototype.compare` functionality.

See [v.12 API Docs](http://nodejs.org/api/buffer.html#buffer_buf_compare_otherbuffer)

```js
  Buffer('123').compare(Buffer('123')); // 0
  Buffer('123').compare(Buffer('1230')); // -1
  Buffer('1230').compare(Buffer('123')); // 1

  Buffer.compare(Buffer('123'), Buffer('123')); // 0
  Buffer.compare(Buffer('123'), Buffer('1230')); // -1
  Buffer.compare(Buffer('1230'), Buffer('123')); // 1
```
