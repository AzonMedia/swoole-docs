# Swoole\Redis

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class Redis
 * @package Swoole
 */
class Redis
{
    /**
     * @var 
     */
    public $onConnect;
    
    /**
     * @var 
     */
    public $onClose;
    
    /**
     * @var 
     */
    public $onMessage;
    
    /**
     * @var 
     */
    public $setting;
    
    /**
     * @var 
     */
    public $host;
    
    /**
     * @var 
     */
    public $port;
    
    /**
     * @var 
     */
    public $sock;
    
    /**
     * @var 
     */
    public $errCode;
    
    /**
     * @var 
     */
    public $errMsg;
    
    
    /**
     * @var integer
     */
    public const STATE_CONNECT = 0;
    
    /**
     * @var integer
     */
    public const STATE_READY = 1;
    
    /**
     * @var integer
     */
    public const STATE_WAIT_RESULT = 2;
    
    /**
     * @var integer
     */
    public const STATE_SUBSCRIBE = 3;
    
    /**
     * @var integer
     */
    public const STATE_CLOSED = 4;
    
    
    /**
     * @param null|array $setting
     * @return void
     */
    public function __construct( ?array $setting) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * @param type $event_name
     * @param type $callback
     * @return void
     */
    public function on( $event_name, $callback) { }
    
    /**
     * @param type $host
     * @param type $port
     * @param type $callback
     * @return void
     */
    public function connect( $host, $port, $callback) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
    /**
     * 
     * @return void
     */
    public function getState( ) { }
    
    /**
     * @param type $command
     * @param type $params
     * @return void
     */
    public function __call( $command, $params) { }
    
}


```

## Examples

