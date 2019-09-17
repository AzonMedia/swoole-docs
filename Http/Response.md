# Swoole\Http\Response

## Intrduction

## API

```php
<?php
namespace Swoole\Http;
/**
 * Class Response
 * @package Swoole\Http
 */
class Response
{
    /**
     * @var 
     */
    public $fd;
    
    /**
     * @var 
     */
    public $header;
    
    /**
     * @var 
     */
    public $cookie;
    
    /**
     * @var 
     */
    public $trailer;
    
    
    
    /**
     * 
     * @return void
     */
    public function initHeader( ) { }
    
    /**
     * @param type name
     * @param type value
     * @param type expires
     * @param type path
     * @param type domain
     * @param type secure
     * @param type httponly
     * @return void
     */
    public function cookie( $name, $value, $expires, $path, $domain, $secure, $httponly) { }
    
    /**
     * @param type name
     * @param type value
     * @param type expires
     * @param type path
     * @param type domain
     * @param type secure
     * @param type httponly
     * @return void
     */
    public function rawcookie( $name, $value, $expires, $path, $domain, $secure, $httponly) { }
    
    /**
     * @param type http_code
     * @param type reason
     * @return void
     */
    public function status( $http_code, $reason) { }
    
    /**
     * @param type compress_level
     * @return void
     */
    public function gzip( $compress_level) { }
    
    /**
     * @param type key
     * @param type value
     * @param type ucwords
     * @return void
     */
    public function header( $key, $value, $ucwords) { }
    
    /**
     * @param type content
     * @return void
     */
    public function write( $content) { }
    
    /**
     * @param type content
     * @return void
     */
    public function end( $content) { }
    
    /**
     * @param type filename
     * @param type offset
     * @param type length
     * @return void
     */
    public function sendfile( $filename, $offset, $length) { }
    
    /**
     * @param type location
     * @param type http_code
     * @return void
     */
    public function redirect( $location, $http_code) { }
    
    /**
     * 
     * @return void
     */
    public function detach( ) { }
    
    /**
     * @param type fd
     * @return void
     */
    public static function create( $fd) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
}


```

## Examples

