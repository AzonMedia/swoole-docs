# Swoole\Atomic\Long

## Intrduction

## API

```php
<?php
namespace Swoole\Atomic;
/**
 * Class Long
 * @package Swoole\Atomic
 */
class Long
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
     * @param type $cmp_value
     * @param type $new_value
     * @return void
     */
    public function cmpset( $cmp_value, $new_value) { }
    
}


```

## Examples

