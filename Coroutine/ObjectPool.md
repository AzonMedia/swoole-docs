# Swoole\Coroutine\ObjectPool

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine;

/**
 * Class ObjectPool
 * @package Swoole\Coroutine
 */
abstract class ObjectPool
{
    /**
     * @var 
     */
    protected static $context;
    
    /**
     * @var 
     */
    protected $object_pool;
    
    /**
     * @var 
     */
    protected $busy_pool;
    
    /**
     * @var 
     */
    protected $type;
    
    
    
    /**
     * @param type $type
     * @param type $pool_size
     * @param type $concurrency
     * @return void
     */
    public function __construct( $type, $pool_size = 10, $concurrency = 10) { }
    
    /**
     * 
     * @return void
     */
    public function get( ) { }
    
    /**
     * 
     * @return void
     */
    public function free( ) { }
    
    /**
     * 
     * @return void
     */
    abstract public function create( ) { }
    
}


```

## Examples

