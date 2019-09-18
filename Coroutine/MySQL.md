# Swoole\Coroutine\MySQL

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine;

/**
 * Class MySQL
 * @package Swoole\Coroutine
 */
class MySQL
{
    /**
     * @var 
     */
    public $serverInfo;
    
    /**
     * @var integer
     */
    public $sock = -1;
    
    /**
     * @var 
     */
    public $connected;
    
    /**
     * @var 
     */
    public $connect_errno;
    
    /**
     * @var 
     */
    public $connect_error;
    
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
     * 
     * @return void
     */
    public function __construct( ) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * 
     * @return void
     */
    public function getDefer( ) { }
    
    /**
     * @param type $defer
     * @return void
     */
    public function setDefer( $defer) { }
    
    /**
     * @param array $server_config
     * @return void
     */
    public function connect( array $server_config) { }
    
    /**
     * @param type $sql
     * @param type $timeout
     * @return void
     */
    public function query( $sql, $timeout) { }
    
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
     * @param type $query
     * @param type $timeout
     * @return void
     */
    public function prepare( $query, $timeout) { }
    
    /**
     * 
     * @return void
     */
    public function recv( ) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function begin( $timeout) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function commit( $timeout) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function rollback( $timeout) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
}


```

## Examples

