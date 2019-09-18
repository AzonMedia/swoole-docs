# Swoole\Coroutine\Http\Server

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine\Http;

/**
 * Class Server
 * @package Swoole\Coroutine\Http
 */
final class Server
{
    /**
     * @var integer
     */
    public $fd = -1;
    
    /**
     * @var 
     */
    public $host;
    
    /**
     * @var integer
     */
    public $port = -1;
    
    /**
     * @var 
     */
    public $ssl;
    
    /**
     * @var 
     */
    public $settings;
    
    /**
     * @var 
     */
    public $errCode;
    
    /**
     * @var 
     */
    public $errMsg;
    
    
    
    /**
     * @param type $host
     * @param type $port
     * @param type $ssl
     * @param type $reuse_port
     * @return void
     */
    public function __construct( $host, $port, $ssl, $reuse_port) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * @param array $settings
     * @return void
     */
    public function set( array $settings) { }
    
    /**
     * @param type $pattern
     * @param callable $callback
     * @return void
     */
    public function handle( $pattern, callable $callback) { }
    
    /**
     * 
     * @return void
     */
    public function onAccept( ) { }
    
    /**
     * 
     * @return void
     */
    public function start( ) { }
    
    /**
     * 
     * @return void
     */
    public function shutdown( ) { }
    
}


```

## Examples

