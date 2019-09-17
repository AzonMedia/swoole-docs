# Swoole\WebSocket\Frame

## Intrduction

## API

```php
<?php
namespace Swoole\WebSocket;
/**
 * Class Frame
 * @package Swoole\WebSocket
 */
class Frame
{
    /**
     * @var 
     */
    public $fd;
    
    /**
     * @var 
     */
    public $data;
    
    /**
     * @var integer
     */
    public $opcode = 1;
    
    /**
     * @var boolean
     */
    public $finish = true;
    
    
    
    /**
     * 
     * @return void
     */
    public function __toString( ) { }
    
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

