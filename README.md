jsfs-api
========

jsfs-api is a JavaScript posix-style file system api designed to be compatible with Node.js and also applicable to other local and remote implementations.

A file system must provide at minimum an implementation for the following methods:

* `mkdir(path, [mode], callback)`
* `readdir(path, callback)`
* `readFile(path, [options], callback)`
* `rename(oldPath, newPath, callback)`
* `rmdir(path, callback)`
* `stat(path, callback)`
* `unlink(path, callback)`
* `writeFile(path, data, [options], callback)`

A file systen can optionally implement the following higher-level methods. If not implemented a default implementation based on the above minimal API is provided.

* `ls(path, [options], callback)`
* `cp(srcpath, dstpath, [options], callback)`
* `mv(srcpath, dstpath, [options], callback)`
* `rm(path, [options], callback)`
* `find(path, expression, [options], callback)`
* `grep(path, pattern, [options], callback)`

