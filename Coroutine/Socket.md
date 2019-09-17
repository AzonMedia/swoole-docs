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
     * @var 
     */
    public $errCode;
    
    
    
    /**
     * @param type domain
     * @param type type
     * @param type protocol
     * @return void
     */
    public function __construct( $domain, $type, $protocol) { }
    
    /**
     * @param type address
     * @param type port
     * @return void
     */
    public function bind( $address, $port) { }
    
    /**
     * @param type backlog
     * @return void
     */
    public function listen( $backlog) { }
    
    /**
     * @param type timeout
     * @return void
     */
    public function accept( $timeout) { }
    
    /**
     * @param type host
     * @param type port
     * @param type timeout
     * @return void
     */
    public function connect( $host, $port, $timeout) { }
    
    /**
     * @param type length
     * @param type timeout
     * @return void
     */
    public function recv( $length, $timeout) { }
    
    /**
     * @param type data
     * @param type timeout
     * @return void
     */
    public function send( $data, $timeout) { }
    
    /**
     * @param type peername
     * @param type timeout
     * @return void
     */
    public function recvfrom( &$peername, $timeout) { }
    
    /**
     * @param type addr
     * @param type port
     * @param type data
     * @return void
     */
    public function sendto( $addr, $port, $data) { }
    
    /**
     * @param type how
     * @return void
     */
    public function shutdown( $how) { }
    
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

