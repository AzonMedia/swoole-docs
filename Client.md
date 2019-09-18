# Swoole\Client

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class Client
 * @package Swoole
 */
class Client
{
    /**
     * @var 
     */
    public $errCode;
    
    /**
     * @var integer
     */
    public $sock = -1;
    
    /**
     * @var 
     */
    public $reuse;
    
    /**
     * @var 
     */
    public $reuseCount;
    
    /**
     * @var 
     */
    public $type;
    
    /**
     * @var 
     */
    public $id;
    
    /**
     * @var 
     */
    public $setting;
    
    /**
     * @var 
     */
    private $onConnect;
    
    /**
     * @var 
     */
    private $onError;
    
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
    private $onBufferFull;
    
    /**
     * @var 
     */
    private $onBufferEmpty;
    
    
    /**
     * @var integer
     */
    public const MSG_OOB = 1;
    
    /**
     * @var integer
     */
    public const MSG_PEEK = 2;
    
    /**
     * @var integer
     */
    public const MSG_DONTWAIT = 64;
    
    /**
     * @var integer
     */
    public const MSG_WAITALL = 256;
    
    /**
     * @var integer
     */
    public const SHUT_RDWR = 2;
    
    /**
     * @var integer
     */
    public const SHUT_RD = 0;
    
    /**
     * @var integer
     */
    public const SHUT_WR = 1;
    
    
    /**
     * @param type $type
     * @param type $async
     * @return void
     */
    public function __construct( $type, $async) { }
    
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
     * @param type $host
     * @param type $port
     * @param type $timeout
     * @param type $sock_flag
     * @return void
     */
    public function connect( $host, $port, $timeout, $sock_flag) { }
    
    /**
     * @param type $size
     * @param type $flag
     * @return void
     */
    public function recv( $size, $flag) { }
    
    /**
     * @param type $data
     * @param type $flag
     * @return void
     */
    public function send( $data, $flag) { }
    
    /**
     * @param type $dst_socket
     * @return void
     */
    public function pipe( $dst_socket) { }
    
    /**
     * @param type $filename
     * @param type $offset
     * @param type $length
     * @return void
     */
    public function sendfile( $filename, $offset, $length) { }
    
    /**
     * @param type $ip
     * @param type $port
     * @param type $data
     * @return void
     */
    public function sendto( $ip, $port, $data) { }
    
    /**
     * 
     * @return void
     */
    public function sleep( ) { }
    
    /**
     * 
     * @return void
     */
    public function wakeup( ) { }
    
    /**
     * 
     * @return void
     */
    public function pause( ) { }
    
    /**
     * 
     * @return void
     */
    public function resume( ) { }
    
    /**
     * @param type $how
     * @return void
     */
    public function shutdown( $how) { }
    
    /**
     * 
     * @return void
     */
    public function isConnected( ) { }
    
    /**
     * 
     * @return void
     */
    public function getsockname( ) { }
    
    /**
     * 
     * @return void
     */
    public function getpeername( ) { }
    
    /**
     * @param type $force
     * @return void
     */
    public function close( $force) { }
    
    /**
     * @param type $event_name
     * @param callable $callback
     * @return void
     */
    public function on( $event_name, callable $callback) { }
    
}


```

## Examples

