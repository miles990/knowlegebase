/*
Title: Base64 Encode Decode in Node.js
*/

## Reference:

* [Wiki](http://zh.wikipedia.org/wiki/Base64)	
* [StackOverflow](http://stackoverflow.com/questions/6182315/how-to-do-base64-encoding-in-node-js)
* [Node.js api doc](http://nodejs.org/docs/latest/api/buffer.html)

<br>


## Example
```
> console.log(new Buffer("Hello World").toString('base64'));
SGVsbG8gV29ybGQ=

> console.log(new Buffer("SGVsbG8gV29ybGQ=", 'base64').toString('ascii'))
Hello World
```
* **'ascii'** - for 7 bit ASCII data only. This encoding method is very fast, and will strip the high bit if set.

* **'utf8'** - Multi byte encoded Unicode characters. Many web pages and other document formats use UTF-8.

* **'ucs2'** - 2-bytes, little endian encoded Unicode characters. It can encode only BMP(Basic Multilingual Plane, U+0000 - U+FFFF).

* **'base64'** - Base64 string encoding.

* **'binary'** - A way of encoding raw binary data into strings by using only the first 8 bits of each character. This encoding method is deprecated and should be avoided in favor of Buffer objects where possible. This encoding will be removed in future versions of Node.