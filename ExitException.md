# Swoole\ExitException

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class ExitException
 * @package Swoole
 */
class ExitException extends \Swoole\Exception
{
    /**
     * @var 
     */
    private $flags;
    
    /**
     * @var 
     */
    private $status;
    
    
    
    /**
     * 
     * @return void
     */
    public function getFlags( ) { }
    
    /**
     * 
     * @return void
     */
    public function getStatus( ) { }
    
}


```

## Examples

