# Swoole\Coroutine\System

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine;

/**
 * Class System
 * @package Swoole\Coroutine
 */
class System
{
    
    
    /**
     * @param type $domain_name
     * @param type $family
     * @param type $timeout
     * @return void
     */
    public static function gethostbyname( $domain_name, $family, $timeout) { }
    
    /**
     * @param type $domain_name
     * @param type $timeout
     * @return void
     */
    public static function dnsLookup( $domain_name, $timeout) { }
    
    /**
     * @param type $command
     * @param type $get_error_stream
     * @return void
     */
    public static function exec( $command, $get_error_stream) { }
    
    /**
     * @param type $seconds
     * @return void
     */
    public static function sleep( $seconds) { }
    
    /**
     * @param type $handle
     * @param type $length
     * @return void
     */
    public static function fread( $handle, $length) { }
    
    /**
     * @param type $handle
     * @param type $string
     * @param type $length
     * @return void
     */
    public static function fwrite( $handle, $string, $length) { }
    
    /**
     * @param type $handle
     * @return void
     */
    public static function fgets( $handle) { }
    
    /**
     * @param type $hostname
     * @param type $family
     * @param type $socktype
     * @param type $protocol
     * @param type $service
     * @param type $timeout
     * @return void
     */
    public static function getaddrinfo( $hostname, $family, $socktype, $protocol, $service, $timeout) { }
    
    /**
     * @param type $filename
     * @return void
     */
    public static function readFile( $filename) { }
    
    /**
     * @param type $filename
     * @param type $data
     * @param type $flags
     * @return void
     */
    public static function writeFile( $filename, $data, $flags) { }
    
    /**
     * @param type $path
     * @return void
     */
    public static function statvfs( $path) { }
    
}


```

## Examples

