# MySQL database access functions without annoying warnings from original repo

## Warning

This extension is deprecated and unmaintained blah blah blah

## Description

This extension provides the mysql family of functions that were provided with
PHP 3-5. These functions have been superseded by MySQLi and PDO_MySQL, which
continue to be bundled with PHP 7.

Although it should be possible to build this extension with PHP 7.0, you are
strongly encouraged to port your code to use either MySQLi or PDO_MySQL, as
this extension is not maintained and is available for historical reasons only.

## Installation
- Clone
- `phpize` (install required dependencies)
- `./configure`
- `make -j3`
- `sudo make install`
- Move created `mysql.so` file (you'd see path to created file) to any place (for example, `/usr/lib/php/7.4/mysql.so`)
- Edit `php.ini` - add compiled library:
```
[mysql]
extension=/usr/lib/php/7.4/mysql.so
```

As I know, it works with PHP8 too
