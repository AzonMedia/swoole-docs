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
     * @param type fd
     * @param type read_callback
     * @param type write_callback
     * @param type events
     * @return void
     */
    public static function add( $fd, $read_callback, $write_callback, $events) { }
    
    /**
     * @param type fd
     * @return void
     */
    public static function del( $fd) { }
    
    /**
     * @param type fd
     * @param type read_callback
     * @param type write_callback
     * @param type events
     * @return void
     */
    public static function set( $fd, $read_callback, $write_callback, $events) { }
    
    /**
     * 
     * @return void
     */
    public static function exit( ) { }
    
    /**
     * @param type fd
     * @param type data
     * @return void
     */
    public static function write( $fd, $data) { }
    
    /**
     * 
     * @return void
     */
    public static function wait( ) { }
    
    /**
     * @param type callback
     * @return void
     */
    public static function defer( $callback) { }
    
    /**
     * @param type callback
     * @param type before
     * @return void
     */
    public static function cycle( $callback, $before) { }
    
}


```

## Examples

