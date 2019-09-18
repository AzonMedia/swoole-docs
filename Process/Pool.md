# Swoole\Process\Pool

## Intrduction

## API

```php
<?php

namespace Swoole\Process;

/**
 * Class Pool
 * @package Swoole\Process
 */
class Pool
{
    /**
     * @var integer
     */
    public $master_pid = -1;
    
    /**
     * @var 
     */
    public $workers;
    
    
    
    /**
     * @param type $worker_num
     * @param type $ipc_type
     * @param type $msgqueue_key
     * @param type $enable_coroutine
     * @return void
     */
    public function __construct( $worker_num, $ipc_type, $msgqueue_key, $enable_coroutine) { }
    
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
     * @param type $event_name
     * @param callable $callback
     * @return void
     */
    public function on( $event_name, callable $callback) { }
    
    /**
     * @param type $worker_id
     * @return void
     */
    public function getProcess( $worker_id) { }
    
    /**
     * @param type $host
     * @param type $port
     * @param type $backlog
     * @return void
     */
    public function listen( $host, $port, $backlog) { }
    
    /**
     * @param type $data
     * @return void
     */
    public function write( $data) { }
    
    /**
     * 
     * @return void
     */
    public function start( ) { }
    
    /**
     * 
     * @return void
     */
    public function shutdown( ) { }
    
}


```

## Examples

