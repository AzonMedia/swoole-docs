# Swoole\Coroutine\Channel

## Intrduction

## API

```php
<?php
namespace Swoole\Coroutine;
/**
 * Class Channel
 * @package Swoole\Coroutine
 */
class Channel
{
    /**
     * @var 
     */
    public $capacity;
    
    /**
     * @var 
     */
    public $errCode;
    
    
    
    /**
     * @param type $size
     * @return void
     */
    public function __construct( $size) { }
    
    /**
     * @param type $data
     * @param type $timeout
     * @return void
     */
    public function push( $data, $timeout) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function pop( $timeout) { }
    
    /**
     * 
     * @return void
     */
    public function isEmpty( ) { }
    
    /**
     * 
     * @return void
     */
    public function isFull( ) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
    /**
     * 
     * @return void
     */
    public function stats( ) { }
    
    /**
     * 
     * @return void
     */
    public function length( ) { }
    
}


```

## Examples

