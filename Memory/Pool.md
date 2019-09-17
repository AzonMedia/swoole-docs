# Swoole\Memory\Pool

## Intrduction

## API

```php
<?php
namespace Swoole\Memory;
/**
 * Class Pool
 * @package Swoole\Memory
 */
class Pool
{
    
    /**
     * @var integer
     */
    public const TYPE_RING = 1;
    
    /**
     * @var integer
     */
    public const TYPE_GLOBAL = 2;
    
    /**
     * @var integer
     */
    public const TYPE_FIXED = 0;
    
    /**
     * @var integer
     */
    public const TYPE_MALLOC = 3;
    
    /**
     * @var integer
     */
    public const TYPE_EMALLOC = 4;
    
    
    /**
     * @param type $size
     * @param type $type
     * @param type $slice_size
     * @param type $shared
     * @return void
     */
    public function __construct( $size, $type, $slice_size, $shared) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * @param type $size
     * @return void
     */
    public function alloc( $size) { }
    
}


```

## Examples

