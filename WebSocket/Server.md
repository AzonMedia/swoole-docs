# Swoole\WebSocket\Server

## Intrduction

## API

```php
<?php

namespace Swoole\WebSocket;

/**
 * Class Server
 * @package Swoole\WebSocket
 */
class Server extends \Swoole\Http\Server
{
    
    
    /**
     * @param type $fd
     * @param type $data
     * @param type $opcode
     * @param type $finish
     * @return void
     */
    public function push( $fd, $data, $opcode, $finish) { }
    
    /**
     * @param type $fd
     * @param type $code
     * @param type $reason
     * @return void
     */
    public function disconnect( $fd, $code, $reason) { }
    
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
     * @return void
     */
    public function isEstablished( $fd) { }
    
    /**
     * @param type $data
     * @param type $opcode
     * @param type $finish
     * @param type $mask
     * @return void
     */
    public static function pack( $data, $opcode, $finish, $mask) { }
    
    /**
     * @param type $data
     * @return void
     */
    public static function unpack( $data) { }
    
}


```

## Examples

