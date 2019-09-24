# Swoole\Runtime

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class Runtime
 * @package Swoole
 */
class Runtime
{
    
    
    /**
     * Deprecated. Will be removed in v4.5.0
     * Will raise a warning if blocking code is used. 
     * @return void
     */
    public static function enableStrictMode( ) { }
    
    /**
     * @param type $enable
     * @param type $flags
     * @return void
     */
    public static function enableCoroutine( $enable, $flags) { }
    
}


```

## Examples

