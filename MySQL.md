# Swoole\MySQL

## Intrduction

## API

```php
<?php
namespace Swoole;
/**
 * Class MySQL
 * @package Swoole
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
    public $errno;
    
    /**
     * @var 
     */
    public $connect_errno;
    
    /**
     * @var 
     */
    public $error;
    
    /**
     * @var 
     */
    public $connect_error;
    
    /**
     * @var 
     */
    public $insert_id;
    
    /**
     * @var 
     */
    public $affected_rows;
    
    /**
     * @var 
     */
    public $onConnect;
    
    /**
     * @var 
     */
    public $onClose;
    
    
    /**
     * @var integer
     */
    public const STATE_QUERY = 0;
    
    /**
     * @var integer
     */
    public const STATE_READ_START = 1;
    
    /**
     * @var integer
     */
    public const STATE_READ_FIELD  = 2;
    
    /**
     * @var integer
     */
    public const STATE_READ_ROW = 3;
    
    /**
     * @var integer
     */
    public const STATE_READ_END = 5;
    
    /**
     * @var integer
     */
    public const STATE_CLOSED = 6;
    
    
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
     * @param array server_config
     * @param type callback
     * @return void
     */
    public function connect( array $server_config, $callback) { }
    
    /**
     * @param type callback
     * @return void
     */
    public function begin( $callback) { }
    
    /**
     * @param type callback
     * @return void
     */
    public function commit( $callback) { }
    
    /**
     * @param type callback
     * @return void
     */
    public function rollback( $callback) { }
    
    /**
     * @param type sql
     * @param type callback
     * @return void
     */
    public function query( $sql, $callback) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
    /**
     * 
     * @return void
     */
    public function getState( ) { }
    
    /**
     * @param type event_name
     * @param type callback
     * @return void
     */
    public function on( $event_name, $callback) { }
    
}


```

## Examples

