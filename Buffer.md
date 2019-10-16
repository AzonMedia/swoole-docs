# Swoole\Buffer

## Intrduction

Allows direct memory manipulation like in C.

**This class will be deprecated.**

## API

```php
<?php

namespace Swoole;

/**
 * Class Buffer
 * Will be deprecated.
 * @package Swoole
 */
class Buffer
{
    /**
     * @var integer
     */
    public $capacity = 128;
    
    /**
     * @var 
     */
    public $length;
    
    
    
    /**
     * @param type $size
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
     * @param type $offset
     * @param type $length
     * @param type $remove
     * @return void
     */
    public function substr( $offset, $length, $remove) { }
    
    /**
     * @param type $offset
     * @param type $data
     * @return void
     */
    public function write( $offset, $data) { }
    
    /**
     * @param type $offset
     * @param type $length
     * @return void
     */
    public function read( $offset, $length) { }
    
    /**
     * @param type $data
     * @return void
     */
    public function append( $data) { }
    
    /**
     * @param type $size
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

