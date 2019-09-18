# Swoole\Timer

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class Timer
 * @package Swoole
 */
class Timer
{
    
    
    /**
     * @param array $settings
     * @return void
     */
    public static function set( array $settings) { }
    
    /**
     * @param type $ms
     * @param callable $callback
     * @param type $params
     * @return void
     */
    public static function tick( $ms, callable $callback, $params) { }
    
    /**
     * @param type $ms
     * @param callable $callback
     * @param type $params
     * @return void
     */
    public static function after( $ms, callable $callback, $params) { }
    
    /**
     * @param type $timer_id
     * @return void
     */
    public static function exists( $timer_id) { }
    
    /**
     * @param type $timer_id
     * @return void
     */
    public static function info( $timer_id) { }
    
    /**
     * 
     * @return void
     */
    public static function stats( ) { }
    
    /**
     * 
     * @return void
     */
    public static function list( ) { }
    
    /**
     * @param type $timer_id
     * @return void
     */
    public static function clear( $timer_id) { }
    
    /**
     * 
     * @return void
     */
    public static function clearAll( ) { }
    
}


```

## Examples

