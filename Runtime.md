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
     * Enables various coroutine hooks.
     * To be used for example to allow the PHP file functions to be nonblocking.
     * @param bool $enable
     * @param int $flags Bitmask of the SWOOLE_HOOK_* constants
     * @return void
     */
    public static function enableCoroutine( $enable, $flags) { }
    
}


```

## Constants

The list of supported constants is:
- SWOOLE_HOOK_TCP - for TCP socket
- SWOOLE_HOOK_UDP - for UDP socket
- SWOOLE_HOOK_UNIX - for UNIX stream socket
- SWOOLE_HOOK_UDG - for UNIX datagram socket
- SWOOLE_HOOK_SSL - for SSL socket
- SWOOLE_HOOK_TLS - for TSL socket
- SWOOLE_HOOK_SLEEP - hook for the \sleep() function
- SWOOLE_HOOK_FILE - for file operations
- SWOOLE_HOOK_STREAM_SELECT - same like SWOOLE_HOOK_STREAM_FUNCTION
- SWOOLE_HOOK_STREAM_FUNCTION - for \stream_select() function
- SWOOLE_HOOK_BLOCKING_FUNCTION - for blocking system calls like \gethostbyname()
- SWOOLE_HOOK_CURL - for curl operations (since Swoole 4.4.0)
- SWOOLE_HOOK_PROC - program execution functions (\proc_open() etc)
- SWOOLE_HOOK_ALL - all of the above

## Examples

Enable the coroutine hooks for sleep() and fread()

```php
<?php
Swoole\Runtime::enableCoroutine(TRUE, SWOOLE_HOOK_SLEEP | SWOOLE_HOOK_FILE);
```
