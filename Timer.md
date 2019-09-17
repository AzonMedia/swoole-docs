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
     * @param type $ms
     * @param type $callback
     * @param type $params
     * @return void
     */
    public static function tick( $ms, $callback, $params) { }
    
    /**
     * @param type $ms
     * @param type $callback
     * @param type $params
     * @return void
     */
    public static function after( $ms, $callback, $params) { }
    
    /**
     * @param type $timer_id
     * @return void
     */
    public static function exists( $timer_id) { }
    
    /**
     * @param type $timer_id
     * @return void
     */
    public static function clear( $timer_id) { }
    
}


```

## Examples

