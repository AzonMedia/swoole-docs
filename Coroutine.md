# Swoole\Coroutine

## Introduction

Swoole provides [coroutines](https://en.wikipedia.org/wiki/Coroutine) - a lightway approach to threading.
It is important to note that the coroutines in Swoole are not executing in parallel - they just do IO operations in parallel.
A worker in Swoole executes only a single coroutine at any given time.

## Details

All details in regards to the coroutine execution and specifics in Swoole along with many examples can be found [here](http://vesko.blogs.azonmedia.com/2019/09/19/coroutines-in-swoole/).

## Options

The following options can be set by providing an associative array to the Coroutine::set() method:
- max_coroutine
- stack_size - the size of the preallocated stack for each coroutine. The default is 8kb.
- log_level
- trace_flags
- socket_connect_timeout
- socket_timeout
- dns_cache_expire
- dns_cache_capacity
- enable_preemptive_scheduler

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
     * Used to set various coroutine related settings 
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
     * Deprecated. 
     * Please use Swoole\Coroutine\System::gethostbyname() instead.
     * @param type $domain_name
     * @param type $family
     * @param type $timeout
     * @return void
     */
    public static function gethostbyname( $domain_name, $family, $timeout) { }
    
    /**
     * Deprecated. 
     * Please use Swoole\Coroutine\System::dnsLookup() instead.
     * @param type $domain_name
     * @param type $timeout
     * @return void
     */
    public static function dnsLookup( $domain_name, $timeout) { }
    
    /**
     * Deprecated. 
     * Please use Swoole\Coroutine\System::exec() instead.
     * @param type $command
     * @param type $get_error_stream
     * @return void
     */
    public static function exec( $command, $get_error_stream) { }
    
    /**
     * Deprecated. 
     * Please use Swoole\Coroutine\System::sleep() instead.
     * @param type $seconds
     * @return void
     */
    public static function sleep( $seconds) { }
    
    /**
     * Deprecated. 
     * Please use Swoole\Coroutine\System::fread() instead.
     * @param type $handle
     * @param type $length
     * @return void
     */
    public static function fread( $handle, $length) { }
    
    /**
     * Deprecated. 
     * Please use Swoole\Coroutine\System::fgets() instead.
     * @param type $handle
     * @return void
     */
    public static function fgets( $handle) { }
    
    /**
     * Deprecated. 
     * Please use Swoole\Coroutine\System::fwrite() instead.
     * @param type $handle
     * @param type $string
     * @param type $length
     * @return void
     */
    public static function fwrite( $handle, $string, $length) { }
    
    /**
     * Deprecated. 
     * Please use Swoole\Coroutine\System::readFile() instead.
     * @param type $filename
     * @return void
     */
    public static function readFile( $filename) { }
    
    /**
     * Deprecated. 
     * Please use Swoole\Coroutine\System::writeFile() instead.
     * @param type $filename
     * @param type $data
     * @param type $flags
     * @return void
     */
    public static function writeFile( $filename, $data, $flags) { }
    
    /**
     * Deprecated.
     * Please use Swoole\Coroutine\System::getaddrinfo() instead.
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
     * Deprecated 
     * Please use Swoole\Coroutine\System::statvfs() instead.
     * @param type $path
     * @return void
     */
    public static function statvfs( $path) { }
    
}

```

## Examples

Executing coroutines in parallel to obtain data from external source by using channels:
```php
<?php
//we want to collect the results from the coroutines so we set the size of the channel to 2
go(function(){
    //the channel can be used only in coroutine context
    //because of this a parent coroutine is needed
    //if this is in the onRequest handler the code would already be in coroutine
    $channel = new Swoole\Coroutine\Channel(2);
    go(function() use ($channel) {
        $mysql = new Swoole\Coroutine\MySQL();
        $mysql->connect([
            'host' => '127.0.0.1',
            'user' => 'user',
            'password' => 'pass',
            'database' => 'testdb',
        ]);
        $data = $mysql->query('select * from menus');
        $channel->push($data);
    });
 
    go(function() use ($channel) {
        $mysql = new Swoole\Coroutine\MySQL();
        $mysql->connect([
            'host' => '127.0.0.1',
            'user' => 'user',
            'password' => 'pass',
            'database' => 'testdb',
        ]);
        $data = $mysql->query('select * from orders');
        $channel->push($data);
    });
 
    $data1 = $channel->pop();
    $data2 = $channel->pop();
 
    //there is no guarantee which result will come first!
    //the returned data needs to be checked (by array keys) or flagged by the sub-coroutines to make sure what is what
    print_r($data1);
    print_r($data2);
 
});
```

And an alternative way of doing the above task by using setDefer() and recv() methods on the MySQL client:
```php
<?php
//for the same of completeness the code is given with server example instead of explicit master coroutine
$Server = new Swoole\Http\Server('0.0.0.0', 8081, SWOOLE_PROCESS);
$Server->on('request', function (\Swoole\Http\Request $SwooleRequest, \Swoole\Http\Response $SwooleResponse) {
//go(function(){ //no need - we are in coroutine context already
    $mysql1 = new Swoole\Coroutine\MySQL();
    $mysql1->connect([
        'host' => '127.0.0.1',
        'user' => 'user',
        'password' => 'pass',
        'database' => 'testdb',
    ]);
    $mysql1->setDefer();
    $mysql1->query('select * from menus');
 
    $mysql2 = new Swoole\Coroutine\MySQL();
    $mysql2->connect([
        'host' => '127.0.0.1',
        'user' => 'user',
        'password' => 'pass',
        'database' => 'testdb',
    ]);
    $mysql2->setDefer();
    $mysql2->query('select * from orders');
 
    $data1 = $mysql1->recv();
    $data2 = $mysql2->recv();
     
    //in this case the order of the data is guaranteed - data1 holds the data from the first connection
    print_r($data1);
    print_r($data2);
    $SwooleResponse->end('ok');
//});
});
$Server->start();
```

Because of the persistent nature of swoole (memory/resources persist between the requests) it is very important to free any allocated resources during execution.
This can be done with defer(). The execution of the deferred functions is in reverse order (as it should be for propres resource deallocation):
```php
<?php
$ConnectionPool = new ConnectionPool();
go(function() use ($ConnectionPool) {
    $Connection = $ConnectionPool->get_connection();
    Swoole\Coroutine::defer(function() use ($Connection) {
        $Connection->free();//this is last
    });
    $Lock = $Connection->obtain_lock();
    defer(function() use ($Lock) {
        $Lock->release();//this is executed first
    });
    //function body
});
```