# Swoole\Server\Task

## Intrduction

## API

```php
<?php
namespace Swoole\Server;
/**
 * Class Task
 * @package Swoole\Server
 */
final class Task
{
    /**
     * @var 
     */
    public $data;
    
    /**
     * @var integer
     */
    public $id = -1;
    
    /**
     * @var integer
     */
    public $worker_id = -1;
    
    /**
     * @var 
     */
    public $flags;
    
    
    
    /**
     * @param type data
     * @return void
     */
    public function finish( $data) { }
    
}


```

## Examples

