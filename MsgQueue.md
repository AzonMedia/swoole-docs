# Swoole\MsgQueue

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class MsgQueue
 * @package Swoole
 */
class MsgQueue
{
    
    
    /**
     * @param type $len
     * @return void
     */
    public function __construct( $len) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * @param type $data
     * @param type $type
     * @return void
     */
    public function push( $data, $type) { }
    
    /**
     * @param type $type
     * @return void
     */
    public function pop( $type) { }
    
    /**
     * @param type $blocking
     * @return void
     */
    public function setBlocking( $blocking) { }
    
    /**
     * 
     * @return void
     */
    public function stats( ) { }
    
    /**
     * 
     * @return void
     */
    public function destroy( ) { }
    
}


```

## Examples

