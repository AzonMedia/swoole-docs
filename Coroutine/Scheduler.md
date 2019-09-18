# Swoole\Coroutine\Scheduler

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine;

/**
 * Class Scheduler
 * @package Swoole\Coroutine
 */
final class Scheduler
{
    /**
     * @var 
     */
    private $_list;
    
    
    
    /**
     * @param callable $func
     * @param type $params
     * @return void
     */
    public function add( callable $func, $params) { }
    
    /**
     * @param type $n
     * @param callable $func
     * @param type $params
     * @return void
     */
    public function parallel( $n, callable $func, $params) { }
    
    /**
     * @param array $settings
     * @return void
     */
    public function set( array $settings) { }
    
    /**
     * 
     * @return void
     */
    public function start( ) { }
    
}


```

## Examples

