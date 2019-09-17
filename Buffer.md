# Swoole\Buffer

## Intrduction

## API

```php
<?php
namespace Swoole;
/**
 * Class Buffer
 * @package Swoole
 */
class Buffer
{
    
    
    /**
     * @param type size
     * @return void
     */
    public function __construct( $size) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * 
     * @return void
     */
    public function __toString( ) { }
    
    /**
     * @param type offset
     * @param type length
     * @param type seek
     * @return void
     */
    public function substr( $offset, $length, $seek) { }
    
    /**
     * @param type offset
     * @param type data
     * @return void
     */
    public function write( $offset, $data) { }
    
    /**
     * @param type offset
     * @param type length
     * @return void
     */
    public function read( $offset, $length) { }
    
    /**
     * @param type data
     * @return void
     */
    public function append( $data) { }
    
    /**
     * @param type size
     * @return void
     */
    public function expand( $size) { }
    
    /**
     * 
     * @return void
     */
    public function recycle( ) { }
    
    /**
     * 
     * @return void
     */
    public function clear( ) { }
    
}


```

## Examples

