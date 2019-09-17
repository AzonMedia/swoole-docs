# Swoole\Redis\Server

## Intrduction

## API

```php
<?php

namespace Swoole\Redis;

/**
 * Class Server
 * @package Swoole\Redis
 */
class Server extends \Swoole\Server
{
    
    /**
     * @var integer
     */
    public const NIL = 1;
    
    /**
     * @var integer
     */
    public const ERROR = 0;
    
    /**
     * @var integer
     */
    public const STATUS = 2;
    
    /**
     * @var integer
     */
    public const INT = 3;
    
    /**
     * @var integer
     */
    public const STRING = 4;
    
    /**
     * @var integer
     */
    public const SET = 5;
    
    /**
     * @var integer
     */
    public const MAP = 6;
    
    
    /**
     * 
     * @return void
     */
    public function start( ) { }
    
    /**
     * @param type $command
     * @param type $callback
     * @param type $number_of_string_param
     * @param type $type_of_array_param
     * @return void
     */
    public function setHandler( $command, $callback, $number_of_string_param, $type_of_array_param) { }
    
    /**
     * @param type $type
     * @param type $value
     * @return void
     */
    public static function format( $type, $value) { }
    
}


```

## Examples

