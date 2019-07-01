# Swoole\Coroutine\Channel

## Documentation

The swoole\coroutine\channel is used to pass data and synchronize between coroutines. It can be created with:
```php
$ch1 = new chan();//this is an alias
$ch2 = new Swoole\Coroutine\Channel($size);
```
The channel is:
- used for communication between Coroutines. If communication between [Workers](../../server/workers/README.md) is needed then [Swoole\Channel](../../memory/channel/README.md) should be used.
- $size = number of elements
- push() does NOT serialize
- pop() is blocking
- push() is blocking
- due to the both pop() and push() being blocking it can be used for synchronization between coroutines.

## API

```php
public function __construct( int $size);
public function push( /* mixed */ $data, int $timeout);

/**
 * It is blocking - until data is provided or the timeout is reached.
* Returns FALSE if the timeout was reached without data being provided.
* Otherwise returns the pushed data.
* @param int $timeout in seconds
* @return mixed
*/
public function pop( int $timeout) /* mixed */;
public function isEmpty();
public function isFull();
public function close();
public function stats();
public function length();
```