# Swoole\Table\Row

## Intrduction

## API

```php
<?php

namespace Swoole\Table;

/**
 * Class Row
 * @package Swoole\Table
 */
class Row implements \ArrayAccess
{
    /**
     * @var 
     */
    public $key;
    
    /**
     * @var 
     */
    public $value;
    
    
    
    /**
     * @param type $offset
     * @return void
     */
    public function offsetExists( $offset) { }
    
    /**
     * @param type $offset
     * @return void
     */
    public function offsetGet( $offset) { }
    
    /**
     * @param type $offset
     * @param type $value
     * @return void
     */
    public function offsetSet( $offset, $value) { }
    
    /**
     * @param type $offset
     * @return void
     */
    public function offsetUnset( $offset) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
}


```

## Examples

