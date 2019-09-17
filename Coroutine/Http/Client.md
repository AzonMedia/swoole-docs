# Swoole\Coroutine\Http\Client

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine\Http;

/**
 * Class Client
 * @package Swoole\Coroutine\Http
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
     * @var 
     */
    public $setting;
    
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
    public $downloadFile;
    
    /**
     * @var 
     */
    public $downloadOffset;
    
    /**
     * @var 
     */
    public $statusCode;
    
    /**
     * @var 
     */
    public $headers;
    
    /**
     * @var 
     */
    public $set_cookie_headers;
    
    /**
     * @var 
     */
    public $cookies;
    
    /**
     * @var 
     */
    public $body;
    
    
    
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
    public function getDefer( ) { }
    
    /**
     * @param type $defer
     * @return void
     */
    public function setDefer( $defer) { }
    
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
     * @return void
     */
    public function execute( $path) { }
    
    /**
     * @param type $path
     * @return void
     */
    public function get( $path) { }
    
    /**
     * @param type $path
     * @param type $data
     * @return void
     */
    public function post( $path, $data) { }
    
    /**
     * @param type $path
     * @param type $file
     * @param type $offset
     * @return void
     */
    public function download( $path, $file, $offset) { }
    
    /**
     * @param type $path
     * @return void
     */
    public function upgrade( $path) { }
    
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
     * @param type $name
     * @param type $type
     * @param type $filename
     * @return void
     */
    public function addData( $path, $name, $type, $filename) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function recv( $timeout) { }
    
    /**
     * @param type $data
     * @param type $opcode
     * @param type $finish
     * @return void
     */
    public function push( $data, $opcode, $finish) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
}


```

## Examples

