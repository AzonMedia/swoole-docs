# Swoole\Http\Request

## Intrduction

## API

```php
<?php

namespace Swoole\Http;

/**
 * Class Request
 * @package Swoole\Http
 */
class Request
{
    /**
     * @var 
     */
    public $fd;
    
    /**
     * @var 
     */
    public $streamId;
    
    /**
     * @var 
     */
    public $header;
    
    /**
     * @var 
     */
    public $server;
    
    /**
     * @var 
     */
    public $cookie;
    
    /**
     * @var 
     */
    public $get;
    
    /**
     * @var 
     */
    public $files;
    
    /**
     * @var 
     */
    public $post;
    
    /**
     * @var 
     */
    public $tmpfiles;
    
    
    
    /**
     * 
     * @return void
     */
    public function rawContent( ) { }
    
    /**
     * 
     * @return void
     */
    public function getData( ) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
}


```

## Examples

