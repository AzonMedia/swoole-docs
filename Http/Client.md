# Swoole\Http\Client

## Intrduction

## API

```php
<?php

namespace Swoole\Http;

/**
 * Class Client
 * @package Swoole\Http
 */
class Client
{
    /**
     * @var 
     */
    public $type;
    
    /**
     * @var 
     */
    public $errCode;
    
    /**
     * @var 
     */
    public $errMsg;
    
    /**
     * @var 
     */
    public $statusCode;
    
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
     * @var 
     */
    public $requestMethod;
    
    /**
     * @var 
     */
    public $requestHeaders;
    
    /**
     * @var 
     */
    public $requestBody;
    
    /**
     * @var 
     */
    public $uploadFiles;
    
    /**
     * @var 
     */
    public $set_cookie_headers;
    
    /**
     * @var 
     */
    public $downloadFile;
    
    /**
     * @var 
     */
    public $headers;
    
    /**
     * @var 
     */
    public $cookies;
    
    /**
     * @var 
     */
    public $body;
    
    /**
     * @var 
     */
    public $onConnect;
    
    /**
     * @var 
     */
    public $onError;
    
    /**
     * @var 
     */
    public $onMessage;
    
    /**
     * @var 
     */
    public $onClose;
    
    
    
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
     * @param type $method
     * @return void
     */
    public function setMethod( $method) { }
    
    /**
     * @param array $headers
     * @return void
     */
    public function setHeaders( array $headers) { }
    
    /**
     * @param array $cookies
     * @return void
     */
    public function setCookies( array $cookies) { }
    
    /**
     * @param type $data
     * @return void
     */
    public function setData( $data) { }
    
    /**
     * @param type $path
     * @param type $name
     * @param type $type
     * @param type $filename
     * @param type $offset
     * @param type $length
     * @return void
     */
    public function addFile( $path, $name, $type, $filename, $offset, $length) { }
    
    /**
     * @param type $path
     * @param type $callback
     * @return void
     */
    public function execute( $path, $callback) { }
    
    /**
     * @param type $data
     * @param type $opcode
     * @param type $finish
     * @return void
     */
    public function push( $data, $opcode, $finish) { }
    
    /**
     * @param type $path
     * @param type $callback
     * @return void
     */
    public function get( $path, $callback) { }
    
    /**
     * @param type $path
     * @param type $data
     * @param type $callback
     * @return void
     */
    public function post( $path, $data, $callback) { }
    
    /**
     * @param type $path
     * @param type $callback
     * @return void
     */
    public function upgrade( $path, $callback) { }
    
    /**
     * @param type $path
     * @param type $file
     * @param type $callback
     * @param type $offset
     * @return void
     */
    public function download( $path, $file, $callback, $offset) { }
    
    /**
     * 
     * @return void
     */
    public function isConnected( ) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
    /**
     * @param type $event_name
     * @param type $callback
     * @return void
     */
    public function on( $event_name, $callback) { }
    
}


```

## Examples

