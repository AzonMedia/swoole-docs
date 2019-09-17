# Swoole\Process

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class Process
 * @package Swoole
 */
class Process
{
    /**
     * @var 
     */
    public $pipe;
    
    /**
     * @var 
     */
    public $callback;
    
    /**
     * @var 
     */
    public $msgQueueId;
    
    /**
     * @var 
     */
    public $msgQueueKey;
    
    /**
     * @var 
     */
    public $pid;
    
    /**
     * @var 
     */
    public $id;
    
    
    /**
     * @var integer
     */
    public const IPC_NOWAIT = 256;
    
    /**
     * @var integer
     */
    public const PIPE_MASTER = 1;
    
    /**
     * @var integer
     */
    public const PIPE_WORKER = 2;
    
    /**
     * @var integer
     */
    public const PIPE_READ = 3;
    
    /**
     * @var integer
     */
    public const PIPE_WRITE = 4;
    
    
    /**
     * @param type $callback
     * @param type $redirect_stdin_and_stdout
     * @param type $pipe_type
     * @return void
     */
    public function __construct( $callback, $redirect_stdin_and_stdout, $pipe_type) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * @param type $blocking
     * @return void
     */
    public static function wait( $blocking) { }
    
    /**
     * @param type $signal_no
     * @param type $callback
     * @return void
     */
    public static function signal( $signal_no, $callback) { }
    
    /**
     * @param type $usec
     * @param type $type
     * @return void
     */
    public static function alarm( $usec, $type) { }
    
    /**
     * @param type $pid
     * @param type $signal_no
     * @return void
     */
    public static function kill( $pid, $signal_no) { }
    
    /**
     * @param type $nochdir
     * @param type $noclose
     * @return void
     */
    public static function daemon( $nochdir, $noclose) { }
    
    /**
     * @param array $cpu_settings
     * @return void
     */
    public static function setaffinity( array $cpu_settings) { }
    
    /**
     * @param type $seconds
     * @return void
     */
    public function setTimeout( $seconds) { }
    
    /**
     * @param type $blocking
     * @return void
     */
    public function setBlocking( $blocking) { }
    
    /**
     * @param type $key
     * @param type $mode
     * @param type $capacity
     * @return void
     */
    public function useQueue( $key, $mode, $capacity) { }
    
    /**
     * 
     * @return void
     */
    public function statQueue( ) { }
    
    /**
     * 
     * @return void
     */
    public function freeQueue( ) { }
    
    /**
     * 
     * @return void
     */
    public function start( ) { }
    
    /**
     * @param type $data
     * @return void
     */
    public function write( $data) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
    /**
     * @param type $size
     * @return void
     */
    public function read( $size) { }
    
    /**
     * @param type $data
     * @return void
     */
    public function push( $data) { }
    
    /**
     * @param type $size
     * @return void
     */
    public function pop( $size) { }
    
    /**
     * @param type $exit_code
     * @return void
     */
    public function exit( $exit_code) { }
    
    /**
     * @param type $exec_file
     * @param type $args
     * @return void
     */
    public function exec( $exec_file, $args) { }
    
    /**
     * @param type $process_name
     * @return void
     */
    public function name( $process_name) { }
    
}


```

## Examples

