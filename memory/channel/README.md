# Swoole Channel


## Documentation

The swoole\channel is used for communication between processes. It is non blocking unlike [swoole\coroutine\channel](../../coroutine/channel/README.md) which is blocking.

- creation - new Swoole\Channel($size)
- used for communication between Workers or processes started with pcntl_fork()
- $size = size in bytes
- push() does serialize
- pop() is non blocking

## API

```php
public function __construct(int $size);
public function __destruct();
public function push( /* mixed */ $data);
public function pop();
public function peek();
public function stats();
```