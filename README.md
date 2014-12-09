#lrn2code
========

An introduction to programming using JavaScript and Node.js

Some notes that need to be fleshed out

1. Installing node.js
  1. On Windows
		1. download from http://nodejs.org
	2. On Mac
		1. ???
	3. On Linux
		1. Ubuntu
			1. apt-get install nodejs
2. Hello World
  1. Hello World from nodejs.org
3. More About JavaScript
  1. Variables
```
var i = 3;
var f = 3.14;
var b = true;
var a = [1, 2, 3];
var o = { first: 1, second: 2 };
```
  2. Operators
    1. Assignment =, +=, -=, etc
	  2. Comparison ==, !=, ===, !==, <, >, <=, >=
	  3. 3 == '3'
	  4. 3 !== '3'
	  5. Arithmetic +, -, *, /, %, ++, --, unary =/-
	  6. Bitwise &, |, ^, ~, <<, >>
	  7. Logical &&, ||, !
	  8. Conditional ? :
	  9. Branches
		  1. if
	  10. Loops
		  1. for
		  2. foreach
		  3. while
	  11. Functions
	  12. Arrays
	  13. Objects

4. The Good Parts are Very Good
  ![The Good Parts](http://ecx.images-amazon.com/images/I/518QVtPWA7L._BO2,204,203,200_PIsitb-sticker-arrow-click,TopRight,35,-76_AA300_SH20_OU01_.jpg)

5. More About node.js
  1. Modules
	  1. http
		2. fs
```		
			var files = fs.readdirSync(dir1);
			var lines = fs.readFileSync(filename, { encoding: "utf8"}).split('\r\n'),
			fs.appendFileSync(out, file2 + '\r\n');
```
		3. path
```
			var fullname = path.resolve(dir1, files1[i1]);
```
		4. querystring
		5. url
	
6. Useful packages
	1. htmlparser2
    1. npm install htmlparser2 -g
```
parser = new htmlparser.Parser({
    onopentag: whenOpenTag,
    ontext: whenText,
    onclosetag: whenCloseTag
  });
```
7. Other helpful code
```
if (!String.prototype.format) {
    String.prototype.format = function () {
        "use strict";

        var args = arguments;
        return this.replace(/\{(\d+)\}/g, function (match, number) {
            var result = args[number] || match;
            return result;
        });
    };
}
```
[http://javascript.crockford.com/tdop/tdop.html](http://javascript.crockford.com/tdop/tdop.html)
