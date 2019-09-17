# Swoole\WebSocket\CloseFrame

## Intrduction

## API

```php
<?php
namespace Swoole\WebSocket;
/**
 * Class CloseFrame
 * @package Swoole\WebSocket
 */
class CloseFrame extends \Swoole\WebSocket\Frame
{
    /**
     * @var integer
     */
    public $opcode = 8;
    
    /**
     * @var integer
     */
    public $code = 1000;
    
    /**
     * @var 
     */
    public $reason;
    
    
    
}


```

## Examples

