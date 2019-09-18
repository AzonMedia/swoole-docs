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
     * @param callable $callback
     * @return void
     */
    public function setHandler( $command, callable $callback) { }
    
    /**
     * @param type $command
     * @return void
     */
    public function getHandler( $command) { }
    
    /**
     * @param type $type
     * @param type $value
     * @return void
     */
    public static function format( $type, $value) { }
    
}


```

## Examples

