# Swoole\Event

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class Event
 * @package Swoole
 */
class Event
{
    
    
    /**
     * @param type $fd
     * @param null|callable $read_callback
     * @param null|callable $write_callback
     * @param type $events
     * @return void
     */
    public static function add( $fd, ?callable $read_callback, ?callable $write_callback, $events) { }
    
    /**
     * @param type $fd
     * @return void
     */
    public static function del( $fd) { }
    
    /**
     * @param type $fd
     * @param null|callable $read_callback
     * @param null|callable $write_callback
     * @param type $events
     * @return void
     */
    public static function set( $fd, ?callable $read_callback, ?callable $write_callback, $events) { }
    
    /**
     * @param type $fd
     * @param type $events
     * @return void
     */
    public static function isset( $fd, $events) { }
    
    /**
     * 
     * @return void
     */
    public static function dispatch( ) { }
    
    /**
     * @param callable $callback
     * @return void
     */
    public static function defer( callable $callback) { }
    
    /**
     * @param null|callable $callback
     * @param type $before
     * @return void
     */
    public static function cycle( ?callable $callback, $before) { }
    
    /**
     * @param type $fd
     * @param type $data
     * @return void
     */
    public static function write( $fd, $data) { }
    
    /**
     * 
     * @return void
     */
    public static function wait( ) { }
    
    /**
     * 
     * @return void
     */
    public static function rshutdown( ) { }
    
    /**
     * 
     * @return void
     */
    public static function exit( ) { }
    
}


```

## Examples

