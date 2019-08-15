# Coroutine Server



## API

#### \Swoole\Coroutine\Server

```php
public funcion __construct(string $host, int $port, bool $ssl)
public funcion set(array $setting)
public funcion handle(callable $fn)
public funcion shutdown()
public funcion start()
```

#### \Swoole\Coroutine\Server\Connection

```php
funcion __construct(Swoole\Coroutine\Socket $conn)
funcion recv( int $timeout)
funcion send( mixed $data)
funcion close()
```
