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
     * @param type worker_num
     * @param type ipc_type
     * @param type msgqueue_key
     * @return void
     */
    public function __construct( $worker_num, $ipc_type, $msgqueue_key) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * @param type event_name
     * @param type callback
     * @return void
     */
    public function on( $event_name, $callback) { }
    
    /**
     * 
     * @return void
     */
    public function getProcess( ) { }
    
    /**
     * @param type host
     * @param type port
     * @param type backlog
     * @return void
     */
    public function listen( $host, $port, $backlog) { }
    
    /**
     * @param type data
     * @return void
     */
    public function write( $data) { }
    
    /**
     * 
     * @return void
     */
    public function start( ) { }
    
}


```

## Examples

