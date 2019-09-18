# Swoole\Coroutine

## Intrduction

## Details

#### Coroutine 

## Options

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
     * Creates a new coroutine and returns a unique ID (cid).
     * The coroutine execution starts immediately 
     * @param callable $func
     * @param array ...$params Optional arguments that will be passed to the callable. 
     * @return int A positive int containing the coroutine ID
     */
    public static function create( callable $func, $params) { }
    
    /**
     * Adds a callable that will be executed at the end of the coroutine execution.
     * To be used for resource deallocation.
     * The registered callbacks are invoked in reverse order as this is the correct order in case resource deallocation is performed.
     * Can be called from within a coroutine. 
     * @param callable $callback
     * @return void
     */
    public static function defer( $callback) { }
    
    /**
     * Used to set vairous coroutine related settings 
     * @param Array $options Associative array like  ['max_coroutine' => 4096]
     * @return void
     */
    public static function set( $options) { }
    
    /**
     * Returns true if the provided coroutine id exists (means is running or suspended).
     * @param int $cid
     * @return bool
     */
    public static function exists( $cid) { }
    
    /**
     * Suspends the coroutine, gives control to the scheduler to run another coroutine.
     * Can be called from within a coroutine. 
     * @return bool
     */
    public static function yield( ) { }
    
    /**
     * Alias of self::yield()
     * @return bool
     */
    public static function suspend( ) { }
    
    /**
     * Resumes the execution of a suspended coroutine.
     * Will raise awarning if the provided $cid dos not exist, its execution is completed or is doing IO (and can not be resumed)
     * "Warning: Swoole\Coroutine::resume(): you can not resume the coroutine which is in IO operation."
     * @param int $cid
     * @return void
     */
    public static function resume( $cid) { }
    
    /**
     * Returns stats about the coroutine execution.
     * Array
     * (
     *     [aio_task_num] => 0
     *     [c_stack_size] => 2097152
     *     [coroutine_num] => 0
     *     [coroutine_peak_num] => 0
     *     [coroutine_last_cid] => 0
     * )
     * @return array
     */
    public static function stats( ) { }
    
    /**
     * Returns the coroutine ID of the current coroutine.
     * If invoked outside a coroutine returns -1. 
     * The coroutine ID is autoincrement. For details @see https://wiki.swoole.com/wiki/page/871.html 
     * @return int Returns -1 or a positive integer between 1 and PHP_INT_MAX
     */
    public static function getCid( ) { }
    
    /**
     * Alias of self::getCid()
     * @return int
     */
    public static function getuid( ) { }
    
    /**
     * Returns the parent coroutine ID of the provided $cid.
     * If no $cid is provided then the parent coroutine of the current one will be returned.
     * If invoked outside coroutine returns FALSE.
     * If there is no parent coroutine returns -1. 
     * @param int|NULL $cid
     * @return int|FALSE
     */
    public static function getPcid( $cid) { }
    
    /**
     * Returns an Swoole\Coroutine\Context object containing the coroutine context of the provided $cid
     * If not $cid is provided the current coroutine is assumed. 
     * Returns NULL if called outside a coroutine and no $cid is provided.
     * @param int $cid
     * @return Swoole\Coroutine\Context|NULL
     */
    public static function getContext( $cid) { }
    
    /**
     * @param type $cid
     * @param type $options
     * @param type $limit
     * @return void
     */
    public static function getBackTrace( $cid, $options, $limit) { }
    
    /**
     * Returns an iterator containing the IDs of the currently running coroutines.
     * @return Swoole\Coroutine\Iterator
     */
    public static function list( ) { }
    
    /**
     * Alias of list()
     * @return void
     */
    public static function listCoroutines( ) { }
    
    /**
     * 
     * @return void
     */
    public static function enableScheduler( ) { }
    
    /**
     * 
     * @return void
     */
    public static function disableScheduler( ) { }
    
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
     * @return void
     */
    public static function fgets( $handle) { }
    
    /**
     * @param type $handle
     * @param type $string
     * @param type $length
     * @return void
     */
    public static function fwrite( $handle, $string, $length) { }
    
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
     * @param type $path
     * @return void
     */
    public static function statvfs( $path) { }
    
}


```

## Examples

