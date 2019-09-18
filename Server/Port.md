# Swoole\Server\Port

## Intrduction

## API

```php
<?php

namespace Swoole\Server;

/**
 * Class Port
 * @package Swoole\Server
 */
class Port
{
    /**
     * @var 
     */
    private $onConnect;
    
    /**
     * @var 
     */
    private $onReceive;
    
    /**
     * @var 
     */
    private $onClose;
    
    /**
     * @var 
     */
    private $onPacket;
    
    /**
     * @var 
     */
    private $onBufferFull;
    
    /**
     * @var 
     */
    private $onBufferEmpty;
    
    /**
     * @var 
     */
    private $onRequest;
    
    /**
     * @var 
     */
    private $onHandShake;
    
    /**
     * @var 
     */
    private $onOpen;
    
    /**
     * @var 
     */
    private $onMessage;
    
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
    public $type;
    
    /**
     * @var integer
     */
    public $sock = -1;
    
    /**
     * @var 
     */
    public $setting;
    
    /**
     * @var 
     */
    public $connections;
    
    
    
    /**
     * 
     * @return void
     */
    private function __construct( ) { }
    
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
     * @param type $event_name
     * @param callable $callback
     * @return void
     */
    public function on( $event_name, callable $callback) { }
    
    /**
     * @param type $event_name
     * @return void
     */
    public function getCallback( $event_name) { }
    
}


```

## Examples

