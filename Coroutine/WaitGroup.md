# Swoole\Coroutine\WaitGroup

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine;

/**
 * Class WaitGroup
 * @package Swoole\Coroutine
 */
class WaitGroup
{
    /**
     * @var 
     */
    protected $chan;
    
    /**
     * @var 
     */
    protected $count;
    
    /**
     * @var 
     */
    protected $waiting;
    
    
    
    /**
     * 
     * @return void
     */
    public function __construct( ) { }
    
    /**
     * @param int $delta
     * @return void
     */
    public function add( int $delta = 1) : void { }
    
    /**
     * 
     * @return void
     */
    public function done( ) : void { }
    
    /**
     * @param float $timeout
     * @return bool
     */
    public function wait( float $timeout = -1) : bool { }
    
}


```

## Examples

