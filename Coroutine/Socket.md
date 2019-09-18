# Swoole\Coroutine\Socket

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine;

/**
 * Class Socket
 * @package Swoole\Coroutine
 */
class Socket
{
    /**
     * @var integer
     */
    public $fd = -1;
    
    /**
     * @var 
     */
    public $errCode;
    
    /**
     * @var 
     */
    public $errMsg;
    
    
    
    /**
     * @param type $domain
     * @param type $type
     * @param type $protocol
     * @return void
     */
    public function __construct( $domain, $type, $protocol) { }
    
    /**
     * @param type $address
     * @param type $port
     * @return void
     */
    public function bind( $address, $port) { }
    
    /**
     * @param type $backlog
     * @return void
     */
    public function listen( $backlog) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function accept( $timeout) { }
    
    /**
     * @param type $host
     * @param type $port
     * @param type $timeout
     * @return void
     */
    public function connect( $host, $port, $timeout) { }
    
    /**
     * @param type $length
     * @param type $timeout
     * @return void
     */
    public function recv( $length, $timeout) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function recvPacket( $timeout) { }
    
    /**
     * @param type $data
     * @param type $timeout
     * @return void
     */
    public function send( $data, $timeout) { }
    
    /**
     * @param type $filename
     * @param type $offset
     * @param type $length
     * @return void
     */
    public function sendFile( $filename, $offset, $length) { }
    
    /**
     * @param type $length
     * @param type $timeout
     * @return void
     */
    public function recvAll( $length, $timeout) { }
    
    /**
     * @param type $data
     * @param type $timeout
     * @return void
     */
    public function sendAll( $data, $timeout) { }
    
    /**
     * @param type $peername
     * @param type $timeout
     * @return void
     */
    public function recvfrom( &$peername, $timeout) { }
    
    /**
     * @param type $addr
     * @param type $port
     * @param type $data
     * @return void
     */
    public function sendto( $addr, $port, $data) { }
    
    /**
     * @param type $level
     * @param type $opt_name
     * @return void
     */
    public function getOption( $level, $opt_name) { }
    
    /**
     * @param array $settings
     * @return void
     */
    public function setProtocol( array $settings) { }
    
    /**
     * @param type $level
     * @param type $opt_name
     * @param type $opt_value
     * @return void
     */
    public function setOption( $level, $opt_name, $opt_value) { }
    
    /**
     * @param type $how
     * @return void
     */
    public function shutdown( $how) { }
    
    /**
     * @param type $event
     * @return void
     */
    public function cancel( $event) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
    /**
     * 
     * @return void
     */
    public function getpeername( ) { }
    
    /**
     * 
     * @return void
     */
    public function getsockname( ) { }
    
}


```

## Examples

