# Swoole\Coroutine

## Intrduction

## API

```php
<?php
namespace Swoole;
/**
 * Class Coroutine
 * @package Swoole
 */
class Coroutine
{
    
    
    /**
     * @param type func
     * @param type params
     * @return void
     */
    public static function create( $func, $params) { }
    
    /**
     * @param type command
     * @return void
     */
    public static function exec( $command) { }
    
    /**
     * @param type domain_name
     * @param type family
     * @param type timeout
     * @return void
     */
    public static function gethostbyname( $domain_name, $family, $timeout) { }
    
    /**
     * @param type callback
     * @return void
     */
    public static function defer( $callback) { }
    
    /**
     * @param type options
     * @return void
     */
    public static function set( $options) { }
    
    /**
     * @param type cid
     * @return void
     */
    public static function exists( $cid) { }
    
    /**
     * 
     * @return void
     */
    public static function yield( ) { }
    
    /**
     * 
     * @return void
     */
    public static function suspend( ) { }
    
    /**
     * @param type cid
     * @return void
     */
    public static function resume( $cid) { }
    
    /**
     * 
     * @return void
     */
    public static function stats( ) { }
    
    /**
     * 
     * @return void
     */
    public static function getCid( ) { }
    
    /**
     * 
     * @return void
     */
    public static function getuid( ) { }
    
    /**
     * 
     * @return void
     */
    public static function getPcid( ) { }
    
    /**
     * @param type seconds
     * @return void
     */
    public static function sleep( $seconds) { }
    
    /**
     * @param type handle
     * @param type length
     * @return void
     */
    public static function fread( $handle, $length) { }
    
    /**
     * @param type handle
     * @return void
     */
    public static function fgets( $handle) { }
    
    /**
     * @param type handle
     * @param type string
     * @param type length
     * @return void
     */
    public static function fwrite( $handle, $string, $length) { }
    
    /**
     * @param type filename
     * @return void
     */
    public static function readFile( $filename) { }
    
    /**
     * @param type filename
     * @param type data
     * @param type flags
     * @return void
     */
    public static function writeFile( $filename, $data, $flags) { }
    
    /**
     * @param type hostname
     * @param type family
     * @param type socktype
     * @param type protocol
     * @param type service
     * @return void
     */
    public static function getaddrinfo( $hostname, $family, $socktype, $protocol, $service) { }
    
    /**
     * @param type path
     * @return void
     */
    public static function statvfs( $path) { }
    
    /**
     * @param type cid
     * @param type options
     * @param type limit
     * @return void
     */
    public static function getBackTrace( $cid, $options, $limit) { }
    
    /**
     * 
     * @return void
     */
    public static function list( ) { }
    
    /**
     * 
     * @return void
     */
    public static function listCoroutines( ) { }
    
}


```

## Examples

