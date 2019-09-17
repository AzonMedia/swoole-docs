# Swoole\Lock

## Intrduction

## API

```php
<?php
namespace Swoole;
/**
 * Class Lock
 * @package Swoole
 */
class Lock
{
    /**
     * @var 
     */
    public $errCode;
    
    
    /**
     * @var integer
     */
    public const FILELOCK = 2;
    
    /**
     * @var integer
     */
    public const MUTEX = 3;
    
    /**
     * @var integer
     */
    public const SEM = 4;
    
    /**
     * @var integer
     */
    public const RWLOCK = 1;
    
    /**
     * @var integer
     */
    public const SPINLOCK = 5;
    
    
    /**
     * @param type type
     * @param type filename
     * @return void
     */
    public function __construct( $type, $filename) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * 
     * @return void
     */
    public function lock( ) { }
    
    /**
     * @param type timeout
     * @return void
     */
    public function lockwait( $timeout) { }
    
    /**
     * 
     * @return void
     */
    public function trylock( ) { }
    
    /**
     * 
     * @return void
     */
    public function lock_read( ) { }
    
    /**
     * 
     * @return void
     */
    public function trylock_read( ) { }
    
    /**
     * 
     * @return void
     */
    public function unlock( ) { }
    
    /**
     * 
     * @return void
     */
    public function destroy( ) { }
    
}


```

## Examples

