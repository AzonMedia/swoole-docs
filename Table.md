# Swoole\Table

## Intrduction

## API

```php
<?php
namespace Swoole;
/**
 * Class Table
 * @package Swoole
 */
class Table implements \Iterator, \ArrayAccess, \Countable
{
    
    /**
     * @var integer
     */
    public const TYPE_INT = 1;
    
    /**
     * @var integer
     */
    public const TYPE_STRING = 7;
    
    /**
     * @var integer
     */
    public const TYPE_FLOAT = 6;
    
    
    /**
     * @param type table_size
     * @param type conflict_proportion
     * @return void
     */
    public function __construct( $table_size, $conflict_proportion) { }
    
    /**
     * @param type name
     * @param type type
     * @param type size
     * @return void
     */
    public function column( $name, $type, $size) { }
    
    /**
     * 
     * @return void
     */
    public function create( ) { }
    
    /**
     * 
     * @return void
     */
    public function destroy( ) { }
    
    /**
     * @param type key
     * @param array value
     * @return void
     */
    public function set( $key, array $value) { }
    
    /**
     * @param type key
     * @param type field
     * @return void
     */
    public function get( $key, $field) { }
    
    /**
     * 
     * @return void
     */
    public function count( ) { }
    
    /**
     * @param type key
     * @return void
     */
    public function del( $key) { }
    
    /**
     * @param type key
     * @return void
     */
    public function exists( $key) { }
    
    /**
     * @param type key
     * @return void
     */
    public function exist( $key) { }
    
    /**
     * @param type key
     * @param type column
     * @param type incrby
     * @return void
     */
    public function incr( $key, $column, $incrby) { }
    
    /**
     * @param type key
     * @param type column
     * @param type decrby
     * @return void
     */
    public function decr( $key, $column, $decrby) { }
    
    /**
     * 
     * @return void
     */
    public function getMemorySize( ) { }
    
    /**
     * @param type offset
     * @return void
     */
    public function offsetExists( $offset) { }
    
    /**
     * @param type offset
     * @return void
     */
    public function offsetGet( $offset) { }
    
    /**
     * @param type offset
     * @param type value
     * @return void
     */
    public function offsetSet( $offset, $value) { }
    
    /**
     * @param type offset
     * @return void
     */
    public function offsetUnset( $offset) { }
    
    /**
     * 
     * @return void
     */
    public function rewind( ) { }
    
    /**
     * 
     * @return void
     */
    public function next( ) { }
    
    /**
     * 
     * @return void
     */
    public function current( ) { }
    
    /**
     * 
     * @return void
     */
    public function key( ) { }
    
    /**
     * 
     * @return void
     */
    public function valid( ) { }
    
}


```

## Examples

