# Swoole\ArrayObject

## Introduction



## API

```php
<?php

namespace Swoole;

/**
 * Class ArrayObject
 * @package Swoole
 */
class ArrayObject implements \ArrayAccess, \Serializable, \Countable, \Iterator
{
    /**
     * @var array
     */
    protected $array;
    
    
    
    /**
     * ArrayObject constructor.
     * @param array $array
     */
    public function __construct( array $array = array (
    )) { }
    
    /**
     * @return bool
     */
    public function isEmpty( ) : bool { }
    
    /**
     * @return int
     */
    public function count( ) : int { }
    
    /**
     * @return mixed
     */
    public function current( ) { }
    
    /**
     * @return mixed
     */
    public function key( ) { }
    
    /**
     * @return bool
     */
    public function valid( ) : bool { }
    
    /**
     * @return mixed
     */
    public function rewind( ) { }
    
    /**
     * @return mixed
     */
    public function next( ) { }
    
    /**
     * @param $key
     * @return ArrayObject|StringObject|mixed
     */
    public function get( $key) { }
    
    /**
     * @param $key
     * @param $value
     * @return $this
     */
    public function set( $key, $value) : self { }
    
    /**
     * @param $key
     * @return $this
     */
    public function delete( $key) : self { }
    
    /**
     * @param $value
     * @param bool $strict
     * @param bool $loop
     * @return $this
     */
    public function remove( $value, bool $strict = true, bool $loop = false) : self { }
    
    /**
     * @return $this
     */
    public function clear( ) : self { }
    
    /**
     * @param mixed $key
     * @return mixed|null
     */
    public function offsetGet( $key) { }
    
    /**
     * @param mixed $key
     * @param mixed $value
     */
    public function offsetSet( $key, $value) { }
    
    /**
     * @param mixed $key
     */
    public function offsetUnset( $key) { }
    
    /**
     * @param mixed $key
     * @return bool
     */
    public function offsetExists( $key) { }
    
    /**
     * @param $key
     * @return bool
     */
    public function exists( $key) : bool { }
    
    /**
     * @param $value
     * @param bool $strict
     * @return bool
     */
    public function contains( $value, bool $strict = true) : bool { }
    
    /**
     * @param $value
     * @param bool $strict
     * @return mixed
     */
    public function indexOf( $value, bool $strict = true) { }
    
    /**
     * @param $value
     * @param bool $strict
     * @return mixed
     */
    public function lastIndexOf( $value, bool $strict = true) { }
    
    /**
     * @param $needle
     * @param $strict
     * @return mixed
     */
    public function search( $needle, $strict = true) { }
    
    /**
     * @param string $glue
     * @return StringObject
     */
    public function join( string $glue = '') : \Swoole\StringObject { }
    
    /**
     * @return StringObject
     */
    public function serialize( ) : \Swoole\StringObject { }
    
    /**
     * @param string $string
     * @return $this
     */
    public function unserialize( $string) : self { }
    
    /**
     * @return float|int
     */
    public function sum( ) { }
    
    /**
     * @return float|int
     */
    public function product( ) { }
    
    /**
     * @param $value
     * @return int
     */
    public function push( $value) { }
    
    /**
     * @param $value
     * @return int
     */
    public function pushBack( $value) { }
    
    /**
     * @param int $offset
     * @param $value
     * @return $this
     */
    public function insert( int $offset, $value) : self { }
    
    /**
     * @return mixed
     */
    public function pop( ) { }
    
    /**
     * @return mixed
     */
    public function popFront( ) { }
    
    /**
     * @param $offset
     * @param int $length
     * @param bool $preserve_keys
     * @return static
     */
    public function slice( $offset, ?int $length = NULL, bool $preserve_keys = false) : self { }
    
    /**
     * @return ArrayObject|StringObject|mixed
     */
    public function randomGet( ) { }
    
    /**
     * @param $fn callable
     * @return $this
     */
    public function each( callable $fn) : self { }
    
    /**
     * @param $fn callable
     * @return static
     */
    public function map( callable $fn) : self { }
    
    /**
     * @param $fn callable
     * @return mixed
     */
    public function reduce( callable $fn) { }
    
    /**
     * @param int $search_value
     * @param bool $strict
     * @return static
     */
    public function keys( ?int $search_value = NULL, $strict = false) : self { }
    
    /**
     * @return static
     */
    public function values( ) : self { }
    
    /**
     * @param $column_key
     * @param mixed ...$index
     * @return static
     */
    public function column( $column_key, $index) : self { }
    
    /**
     * @param int $sort_flags
     * @return static
     */
    public function unique( int $sort_flags = Swoole\SORT_STRING) : self { }
    
    /**
     * @param bool $preserve_keys
     * @return static
     */
    public function reverse( bool $preserve_keys = false) : self { }
    
    /**
     * @param int $size
     * @param bool $preserve_keys
     * @return static
     */
    public function chunk( int $size, bool $preserve_keys = false) : self { }
    
    /**
     * Swap keys and values in an array
     * @return static
     */
    public function flip( ) : self { }
    
    /**
     * @param $fn callable
     * @param int $flag
     * @return static
     */
    public function filter( callable $fn, int $flag = 0) : self { }
    
    /**
     * @param int $sort_order
     * @param int $sort_flags
     * @return $this
     */
    public function multiSort( int $sort_order = Swoole\SORT_ASC, int $sort_flags = Swoole\SORT_REGULAR) : self { }
    
    /**
     * @param int $sort_flags
     * @return $this
     */
    public function asort( int $sort_flags = Swoole\SORT_REGULAR) : self { }
    
    /**
     * @param int $sort_flags
     * @return $this
     */
    public function arsort( int $sort_flags = Swoole\SORT_REGULAR) : self { }
    
    /**
     * @param int $sort_flags
     * @return $this
     */
    public function krsort( int $sort_flags = Swoole\SORT_REGULAR) : self { }
    
    /**
     * @param int $sort_flags
     * @return $this
     */
    public function ksort( int $sort_flags = Swoole\SORT_REGULAR) : self { }
    
    /**
     * @return $this
     */
    public function natcasesort( ) : self { }
    
    /**
     * @return $this
     */
    public function natsort( ) : self { }
    
    /**
     * @param int $sort_flags
     * @return $this
     */
    public function rsort( int $sort_flags = Swoole\SORT_REGULAR) : self { }
    
    /**
     * @return $this
     */
    public function shuffle( ) : self { }
    
    /**
     * @param int $sort_flags
     * @return $this
     */
    public function sort( int $sort_flags = Swoole\SORT_REGULAR) : self { }
    
    /**
     * @param callable $value_compare_func
     * @return $this
     */
    public function uasort( callable $value_compare_func) : self { }
    
    /**
     * @param callable $value_compare_func
     * @return $this
     */
    public function uksort( callable $value_compare_func) : self { }
    
    /**
     * @param callable $value_compare_func
     * @return $this
     */
    public function usort( callable $value_compare_func) : self { }
    
    /**
     * @return array
     */
    public function __toArray( ) : array { }
    
    /**
     * @param $value
     * @return ArrayObject|StringObject|mixed
     */
    protected static function detectType( $value) { }
    
    /**
     * @param string $value
     * @return StringObject
     */
    protected static function detectStringType( string $value) : \Swoole\StringObject { }
    
    /**
     * @param array $value
     * @return static
     */
    protected static function detectArrayType( array $value) : self { }
    
}


```

## Examples

