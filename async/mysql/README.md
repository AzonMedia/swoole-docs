# Swoole Mysql

This is an async mysql client. For coroutine mysql client see [swoole\coroutine\mysql](../../coroutine/mysql/README.md).

## API
```php
public function __construct();
public function __destruct();
public function connect(array $server_config, callable $callback);
public function begin( callable $callback);
public function commit( callable $callback);
public function rollback( callable $callback);
public function query( string $sql, callable $callback);
public function close();
public function getState();
public function on( string $event_name, callable $callback);

```