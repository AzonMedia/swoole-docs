# Swoole\Coroutine\Server

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine;

/**
 * Class Server
 * @package Swoole\Coroutine
 */
class Server
{
    /** @var string */
    public $host;
    
    /** @var int */
    public $port;
    
    /** @var int */
    public $type = 2;
    
    /** @var int */
    public $fd = -1;
    
    /** @var int */
    public $errCode;
    
    /** @var array */
    public $setting;
    
    /** @var bool */
    protected $running;
    
    /** @var callable|null */
    protected $fn;
    
    /** @var Socket */
    protected $socket;
    
    
    
    /**
         * Server constructor.
         * @param string $host
         * @param int $port
         * @param bool $ssl
         * @param bool $reuse_port
         * @throws Exception
         */
    public function __construct( string $host, int $port = 0, bool $ssl = false, bool $reuse_port = false) { }
    
    /**
     * @param array $setting
     * @return void
     */
    public function set( array $setting) : void { }
    
    /**
     * @param callable $fn
     * @return void
     */
    public function handle( callable $fn) : void { }
    
    /**
     * 
     * @return bool
     */
    public function shutdown( ) : bool { }
    
    /**
     * 
     * @return bool
     */
    public function start( ) : bool { }
    
}


```

## Examples

