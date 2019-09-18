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
    public $id;
    
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
     * @param type $timeout
     * @return void
     */
    public function fetch( $timeout) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function fetchAll( $timeout) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function nextResult( $timeout) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function recv( $timeout) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
}


```

## Examples

