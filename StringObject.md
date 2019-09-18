# Swoole\StringObject

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class StringObject
 * @package Swoole
 */
class StringObject
{
    /**
         * @var string
         */
    protected $string;
    
    
    
    /**
         * StringObject constructor.
         * @param $string
         */
    public function __construct( string $string = '') { }
    
    /**
         * @return int
         */
    public function length( ) : int { }
    
    /**
         * @param string $needle
         * @param int $offset
         * @return bool|int
         */
    public function indexOf( string $needle, int $offset = 0) { }
    
    /**
         * @param string $needle
         * @param int $offset
         * @return bool|int
         */
    public function lastIndexOf( string $needle, int $offset = 0) { }
    
    /**
         * @param string $needle
         * @param int $offset
         * @return bool|int
         */
    public function pos( string $needle, int $offset = 0) { }
    
    /**
         * @param string $needle
         * @param int $offset
         * @return bool|int
         */
    public function rpos( string $needle, int $offset = 0) { }
    
    /**
         * @param string $needle
         * @return bool|int
         */
    public function ipos( string $needle) { }
    
    /**
         * @return static
         */
    public function lower( ) : \self { }
    
    /**
         * @return static
         */
    public function upper( ) : \self { }
    
    /**
         * @return static
         */
    public function trim( ) : \self { }
    
    /**
         * @return static
         */
    public function lrim( ) : \self { }
    
    /**
         * @return static
         */
    public function rtrim( ) : \self { }
    
    /**
         * @param int $offset
         * @param mixed ...$length
         * @return static
         */
    public function substr( int $offset, $length) : \self { }
    
    /**
         * @param $n
         * @return StringObject
         */
    public function repeat( $n) { }
    
    /**
         * @param string $search
         * @param string $replace
         * @param null $count
         * @return static
         */
    public function replace( string $search, string $replace, &$count = NULL) : \self { }
    
    /**
         * @param string $needle
         * @return bool
         */
    public function startsWith( string $needle) : bool { }
    
    /**
         * @param string $subString
         * @return bool
         */
    public function contains( string $subString) : bool { }
    
    /**
         * @param string $needle
         * @return bool
         */
    public function endsWith( string $needle) : bool { }
    
    /**
         * @param string $delimiter
         * @param int $limit
         * @return ArrayObject
         */
    public function split( string $delimiter, int $limit = Swoole\PHP_INT_MAX) : \Swoole\ArrayObject { }
    
    /**
         * @param int $index
         * @return string
         */
    public function char( int $index) : string { }
    
    /**
         * @param int $chunkLength
         * @param string $chunkEnd
         * @return static
         */
    public function chunkSplit( int $chunkLength = 1, string $chunkEnd = '') : \self { }
    
    /**
         * @param int $splitLength
         * @return ArrayObject
         */
    public function chunk( $splitLength = 1) : \Swoole\ArrayObject { }
    
    /**
         * @return string
         */
    public function toString( ) { }
    
    /**
         * @return string
         */
    public function __toString( ) : string { }
    
    /**
         * @param array $value
         * @return ArrayObject
         */
    protected static function detectArrayType( array $value) : \Swoole\ArrayObject { }
    
}


```

## Examples

