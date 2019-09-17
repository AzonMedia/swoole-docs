# Swoole\Async

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class Async
 * @package Swoole
 */
class Async
{
    
    
    /**
     * @param type $filename
     * @param type $callback
     * @param type $chunk_size
     * @param type $offset
     * @return void
     */
    public static function read( $filename, $callback, $chunk_size, $offset) { }
    
    /**
     * @param type $filename
     * @param type $content
     * @param type $offset
     * @param type $callback
     * @return void
     */
    public static function write( $filename, $content, $offset, $callback) { }
    
    /**
     * @param type $filename
     * @param type $callback
     * @return void
     */
    public static function readFile( $filename, $callback) { }
    
    /**
     * @param type $filename
     * @param type $content
     * @param type $callback
     * @param type $flags
     * @return void
     */
    public static function writeFile( $filename, $content, $callback, $flags) { }
    
    /**
     * @param type $hostname
     * @param type $callback
     * @return void
     */
    public static function dnsLookup( $hostname, $callback) { }
    
    /**
     * @param type $domain_name
     * @param type $timeout
     * @return void
     */
    public static function dnsLookupCoro( $domain_name, $timeout) { }
    
    /**
     * @param array $settings
     * @return void
     */
    public static function set( array $settings) { }
    
    /**
     * @param type $command
     * @param type $callback
     * @return void
     */
    public static function exec( $command, $callback) { }
    
}


```

## Examples

