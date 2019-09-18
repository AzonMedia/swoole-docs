# Swoole\Coroutine\Server\Connection

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine\Server;

/**
 * Class Connection
 * @package Swoole\Coroutine\Server
 */
class Connection
{
    /**
     * @var 
     */
    public $socket;
    
    
    
    /**
     * @param \Swoole\Coroutine\Socket $conn
     * @return void
     */
    public function __construct( \Swoole\Coroutine\Socket $conn) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function recv( $timeout = 0) { }
    
    /**
     * @param type $data
     * @return void
     */
    public function send( $data) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
}


```

## Examples

