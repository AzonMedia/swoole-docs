# Swoole\Coroutine\Client

## Intrduction

## API

```php
<?php
namespace Swoole\Coroutine;
/**
 * Class Client
 * @package Swoole\Coroutine
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
    public $type;
    
    /**
     * @var 
     */
    public $setting;
    
    /**
     * @var 
     */
    public $connected;
    
    
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
     * @param type type
     * @return void
     */
    public function __construct( $type) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * @param array settings
     * @return void
     */
    public function set( array $settings) { }
    
    /**
     * @param type host
     * @param type port
     * @param type timeout
     * @param type sock_flag
     * @return void
     */
    public function connect( $host, $port, $timeout, $sock_flag) { }
    
    /**
     * @param type timeout
     * @return void
     */
    public function recv( $timeout) { }
    
    /**
     * @param type length
     * @return void
     */
    public function peek( $length) { }
    
    /**
     * @param type data
     * @return void
     */
    public function send( $data) { }
    
    /**
     * @param type filename
     * @param type offset
     * @param type length
     * @return void
     */
    public function sendfile( $filename, $offset, $length) { }
    
    /**
     * @param type address
     * @param type port
     * @param type data
     * @return void
     */
    public function sendto( $address, $port, $data) { }
    
    /**
     * @param type length
     * @param type address
     * @param type port
     * @return void
     */
    public function recvfrom( $length, &$address, &$port) { }
    
    /**
     * 
     * @return void
     */
    public function enableSSL( ) { }
    
    /**
     * 
     * @return void
     */
    public function getPeerCert( ) { }
    
    /**
     * 
     * @return void
     */
    public function verifyPeerCert( ) { }
    
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
     * 
     * @return void
     */
    public function close( ) { }
    
}


```

## Examples

