# Swoole Coroutine Mysql

## Documentation

swoole\coroutine\mysql is a coroutine based mysql client. For an async mysql client see [swoole\mysql](../../async/mysql/README.md).

"swoole_server and swoole_http_server create one coroutine for each request, then maintain and schedule the request based on client side IO status within swoole_server and swoole_http_server."

This means that if in on('Request'):

- mysqli is used this will block the whole worker process until the queries are executed
- if Swoole\Coroutine\Mysql is used this will NOT block the worker
- if Swoole\Coroutine\Mysql->setDefer() and Swoole\Coroutine\Mysql->revc() is used then it is possible to use two simultaneous Swoole\Coroutine\Mysql connections to retrieve data simultaneously:

```php
$start = time();
$swoole_mysql1->query('select sleep(5)');
$swoole_mysql2->query('select sleep(5)');
$ret1 = $swoole_mysql1->recv();
$ret2 = $swoole_mysql2->recv();
$end = time();
print $end - $start;//prints 5 not 10
```

## API

#### swoole\coroutine\mysql

```php
public $serverInfo;
public $sock;
public $connected;
public $connect_error;
public $connect_errno;
public $affected_rows;
public $insert_id;
public $error;
public $errno;

public function __construct();
public function __destruct();
public function connect(array $server_config);
public function query( string $sql, int $timeout) : array;
public function recv();
public function nextResult();
public function begin( int $timeout);
public function commit( int $timeout);
public function rollback( int $timeout);
public function prepare( string $query, int $timeout) /* Swoole\Coroutine\MySQL\Statement | bool */;
public function setDefer( bool $defer);
public function getDefer();
public function close();
```

#### swoole\coroutine\mysql\statement

```php
public $affected_rows;
public $insert_id;
public $error;
public $errno;

/**
 * Executes the statement and returns all the result.
 * No fetchAll() is possible after that.
 * @param array $params Associative array with parameters to be bound in the query
 * @param int $timeout
 * @return Two dimensional array with results or boolean if the queyr is not a SELECT
 */
public  function execute( array $params, int $timeout) /* bool|array */;
public  function fetch();
public  function fetchAll() : array;
public  function nextResult();
public  function __destruct();
```