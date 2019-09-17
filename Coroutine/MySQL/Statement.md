# Swoole\Coroutine\MySQL\Statement

## Intrduction

## API

```php
<?php
namespace Swoole\Coroutine\MySQL;
/**
 * Class Statement
 * @package Swoole\Coroutine\MySQL
 */
class Statement
{
    /**
     * @var 
     */
    public $affected_rows;
    
    /**
     * @var 
     */
    public $insert_id;
    
    /**
     * @var 
     */
    public $error;
    
    /**
     * @var 
     */
    public $errno;
    
    
    
    /**
     * @param type $params
     * @param type $timeout
     * @return void
     */
    public function execute( $params, $timeout) { }
    
    /**
     * 
     * @return void
     */
    public function fetch( ) { }
    
    /**
     * 
     * @return void
     */
    public function fetchAll( ) { }
    
    /**
     * 
     * @return void
     */
    public function nextResult( ) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
}


```

## Examples

