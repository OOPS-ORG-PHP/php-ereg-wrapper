Wrapper for PHP ereg extension
===============================
[![GitHub license](https://img.shields.io/badge/license-BSD-blue.svg?style=plastic)](https://raw.githubusercontent.com/OOPS-ORG-PHP/php-ereg-wrapper/master/LICENSE)

The ereg-wrapper api support ereg extension api, and was designed to work best as with ereg extension.
If you have PHP7 environment and must need removed ereg extension api, this is good choise.


## License
BSD 2-clause

## Requirements

1. PHP 7.0.0 and after

## SYNOPSIS

***ereg*** : http://php.net/manual/en/function.ereg.php
```php
int ereg ( string $pattern , string $string [, array &$regs ] )
```

***eregi*** : http://php.net/manual/en/function.eregi.php
```php
int eregi ( string $pattern , string $string [, array &$regs ] )
```

***ereg_replace*** : http://php.net/manual/en/function.ereg-replace.php
```php
string ereg_replace ( string $pattern , string $replacement , string $string )
```

***eregi_replace*** : http://php.net/manual/en/function.eregi-replace.php
```php
string eregi_replace ( string $pattern , string $replacement , string $string )
```

***split*** : http://php.net/manual/en/function.split.php
```php
array split ( string $pattern , string $string [, int $limit = -1 ] )
```

***spliti*** : http://php.net/manual/en/function.spliti.php
```php
array spliti ( string $pattern , string $string [, int $limit = -1 ] )
```

***sql_regcase*** : http://php.net/manual/en/function.sql-regcase.php
```php
string sql_regcase ( string $string )
```

## Example
```php
<?php
# even if loaded ereg extension, well done.
require_once 'ereg-wrapper.php';

if ( ! ereg ('a', 'aaa') )
    echo 'not ';
echo "matched\n";

if ( ! eregi ('A', 'aaa') )
    echo 'not ';
echo "matched\n";
?>
```

## Credits
JoungKyun.Kim
