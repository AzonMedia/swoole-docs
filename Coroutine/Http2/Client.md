# Swoole\Coroutine\Http2\Client

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine\Http2;

/**
 * Class Client
 * @package Swoole\Coroutine\Http2
 */
class Client
{
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
    public $ssl;
    
    
    
    /**
     * @param type $host
     * @param type $port
     * @param type $ssl
     * @return void
     */
    public function __construct( $host, $port, $ssl) { }
    
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
     * 
     * @return void
     */
    public function connect( ) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function stats( $key) { }
    
    /**
     * @param type $stream_id
     * @return void
     */
    public function isStreamExist( $stream_id) { }
    
    /**
     * @param type $request
     * @return void
     */
    public function send( $request) { }
    
    /**
     * @param type $stream_id
     * @param type $data
     * @param type $end_stream
     * @return void
     */
    public function write( $stream_id, $data, $end_stream) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function recv( $timeout) { }
    
    /**
     * @param type $error_code
     * @param type $debug_data
     * @return void
     */
    public function goaway( $error_code, $debug_data) { }
    
    /**
     * 
     * @return void
     */
    public function ping( ) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
}


```

## Examples

