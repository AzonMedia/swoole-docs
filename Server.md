# Swoole\Server

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class Server
 * @package Swoole
 */
class Server
{
    /**
     * @var 
     */
    private $onStart;
    
    /**
     * @var 
     */
    private $onShutdown;
    
    /**
     * @var 
     */
    private $onWorkerStart;
    
    /**
     * @var 
     */
    private $onWorkerStop;
    
    /**
     * @var 
     */
    private $onWorkerExit;
    
    /**
     * @var 
     */
    private $onWorkerError;
    
    /**
     * @var 
     */
    private $onTask;
    
    /**
     * @var 
     */
    private $onFinish;
    
    /**
     * @var 
     */
    private $onManagerStart;
    
    /**
     * @var 
     */
    private $onManagerStop;
    
    /**
     * @var 
     */
    private $onPipeMessage;
    
    /**
     * @var 
     */
    public $setting;
    
    /**
     * @var 
     */
    public $connections;
    
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
    public $type;
    
    /**
     * @var 
     */
    public $mode;
    
    /**
     * @var 
     */
    public $ports;
    
    /**
     * @var 
     */
    public $master_pid;
    
    /**
     * @var 
     */
    public $manager_pid;
    
    /**
     * @var integer
     */
    public $worker_id = -1;
    
    /**
     * @var 
     */
    public $taskworker;
    
    /**
     * @var 
     */
    public $worker_pid;
    
    
    
    /**
     * @param type $host
     * @param type $port
     * @param type $mode
     * @param type $sock_type
     * @return void
     */
    public function __construct( $host, $port, $mode, $sock_type) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * @param type $host
     * @param type $port
     * @param type $sock_type
     * @return void
     */
    public function listen( $host, $port, $sock_type) { }
    
    /**
     * @param type $host
     * @param type $port
     * @param type $sock_type
     * @return void
     */
    public function addlistener( $host, $port, $sock_type) { }
    
    /**
     * @param type $event_name
     * @param callable $callback
     * @return void
     */
    public function on( $event_name, callable $callback) { }
    
    /**
     * @param type $event_name
     * @return void
     */
    public function getCallback( $event_name) { }
    
    /**
     * @param array $settings
     * @return void
     */
    public function set( array $settings) { }
    
    /**
     * 
     * @return void
     */
    public function start( ) { }
    
    /**
     * @param type $fd
     * @param type $send_data
     * @param type $server_socket
     * @return void
     */
    public function send( $fd, $send_data, $server_socket) { }
    
    /**
     * @param type $ip
     * @param type $port
     * @param type $send_data
     * @param type $server_socket
     * @return void
     */
    public function sendto( $ip, $port, $send_data, $server_socket) { }
    
    /**
     * @param type $conn_fd
     * @param type $send_data
     * @return void
     */
    public function sendwait( $conn_fd, $send_data) { }
    
    /**
     * @param type $fd
     * @return void
     */
    public function exists( $fd) { }
    
    /**
     * @param type $fd
     * @return void
     */
    public function exist( $fd) { }
    
    /**
     * @param type $fd
     * @param type $is_protected
     * @return void
     */
    public function protect( $fd, $is_protected) { }
    
    /**
     * @param type $conn_fd
     * @param type $filename
     * @param type $offset
     * @param type $length
     * @return void
     */
    public function sendfile( $conn_fd, $filename, $offset, $length) { }
    
    /**
     * @param type $fd
     * @param type $reset
     * @return void
     */
    public function close( $fd, $reset) { }
    
    /**
     * @param type $fd
     * @return void
     */
    public function confirm( $fd) { }
    
    /**
     * @param type $fd
     * @return void
     */
    public function pause( $fd) { }
    
    /**
     * @param type $fd
     * @return void
     */
    public function resume( $fd) { }
    
    /**
     * @param type $data
     * @param type $worker_id
     * @param null|callable $finish_callback
     * @return void
     */
    public function task( $data, $worker_id, ?callable $finish_callback) { }
    
    /**
     * @param type $data
     * @param type $timeout
     * @param type $worker_id
     * @return void
     */
    public function taskwait( $data, $timeout, $worker_id) { }
    
    /**
     * @param array $tasks
     * @param type $timeout
     * @return void
     */
    public function taskWaitMulti( array $tasks, $timeout) { }
    
    /**
     * @param array $tasks
     * @param type $timeout
     * @return void
     */
    public function taskCo( array $tasks, $timeout) { }
    
    /**
     * @param type $data
     * @return void
     */
    public function finish( $data) { }
    
    /**
     * 
     * @return void
     */
    public function reload( ) { }
    
    /**
     * 
     * @return void
     */
    public function shutdown( ) { }
    
    /**
     * @param type $worker_id
     * @return void
     */
    public function stop( $worker_id) { }
    
    /**
     * 
     * @return void
     */
    public function getLastError( ) { }
    
    /**
     * @param type $reactor_id
     * @return void
     */
    public function heartbeat( $reactor_id) { }
    
    /**
     * @param type $fd
     * @param type $reactor_id
     * @return void
     */
    public function getClientInfo( $fd, $reactor_id) { }
    
    /**
     * @param type $start_fd
     * @param type $find_count
     * @return void
     */
    public function getClientList( $start_fd, $find_count) { }
    
    /**
     * @param type $fd
     * @param type $reactor_id
     * @return void
     */
    public function connection_info( $fd, $reactor_id) { }
    
    /**
     * @param type $start_fd
     * @param type $find_count
     * @return void
     */
    public function connection_list( $start_fd, $find_count) { }
    
    /**
     * @param type $message
     * @param type $dst_worker_id
     * @return void
     */
    public function sendMessage( $message, $dst_worker_id) { }
    
    /**
     * @param \swoole_process $process
     * @return void
     */
    public function addProcess( \swoole_process $process) { }
    
    /**
     * 
     * @return void
     */
    public function stats( ) { }
    
    /**
     * @param type $fd
     * @param type $uid
     * @return void
     */
    public function bind( $fd, $uid) { }
    
}


```

## Examples

