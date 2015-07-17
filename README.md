filesearch (ls | grep)
======================

Utility for file searching - Search a directory for files that match a given string.

Install
-------
 	npm install -g novac182-filesearch

Usage
-----

   * `filesearch matchString`

Core Code
---------

```js
var exec = require('child_process').exec;
var child = exec('ls | grep ' + searchPattern, function(err, stdout, stderr){
	console.log(stdout);
});
```
