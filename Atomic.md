# Swoole\Atomic

## Intrduction

## API

```php
<?php
namespace Swoole;
/**
 * Class Atomic
 * @package Swoole
 */
class Atomic
{
    
    
    /**
     * @param type $value
     * @return void
     */
    public function __construct( $value) { }
    
    /**
     * @param type $add_value
     * @return void
     */
    public function add( $add_value) { }
    
    /**
     * @param type $sub_value
     * @return void
     */
    public function sub( $sub_value) { }
    
    /**
     * 
     * @return void
     */
    public function get( ) { }
    
    /**
     * @param type $value
     * @return void
     */
    public function set( $value) { }
    
    /**
     * @param type $timeout
     * @return void
     */
    public function wait( $timeout) { }
    
    /**
     * @param type $count
     * @return void
     */
    public function wakeup( $count) { }
    
    /**
     * @param type $cmp_value
     * @param type $new_value
     * @return void
     */
    public function cmpset( $cmp_value, $new_value) { }
    
}


```

## Examples

