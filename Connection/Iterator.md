# Swoole\Connection\Iterator

## Intrduction

## API

```php
<?php
namespace Swoole\Connection;
/**
 * Class Iterator
 * @package Swoole\Connection
 */
class Iterator implements \Iterator, \ArrayAccess, \Countable
{
    
    
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
    
    /**
     * 
     * @return void
     */
    public function count( ) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * @param type $fd
     * @return void
     */
    public function offsetExists( $fd) { }
    
    /**
     * @param type $fd
     * @return void
     */
    public function offsetGet( $fd) { }
    
    /**
     * @param type $fd
     * @param type $value
     * @return void
     */
    public function offsetSet( $fd, $value) { }
    
    /**
     * @param type $fd
     * @return void
     */
    public function offsetUnset( $fd) { }
    
}


```

## Examples

