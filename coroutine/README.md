# Swoole Coroutine

## Subsections
- [Coroutine\Channel](./channel/README.md)
- [Coroutine\Mysql](./mysql/README.md)
- [Coroutine\Server](./server/README.md)
- [Coroutine\Socket](./server/README.md)

## Documentation

#### Aliases

- \Go - \Swoole\Coroutine::Create()
- \Co - \Swoole\Coroutine (this allows to access the coroutine clients like \Co\Mysql instead of \Swoole\Coroutines\Mysql)
- \chan - \Swoole\Coroutine\Channel

## API

```php
/**
 * Creates a new coroutine and returns a unique ID (cid).
 * This cid can be used to resume to coroutine with resume($cid)
 * @param callable $func
 * @param array $params
 * @return int
 */
public static function create( callable $func, array $params) : int;

/**
 * Executes a command from the shell/OS.
 * Retruns an array in format $ret['code'] => int, $ret['signal'] => int, $ret['output'] => string
 * @param string $command
 * @return array
 */
public static function exec( string $command) : array;
public static function gethostbyname( $domain_name,  $family,  $timeout);
public static function defer( $callback);
public static function set( $options);

/**
 * Returns TRUE only if the coroutine is still executing (or it is suspended)
 * @param int $cid
 * @return bool
 */
public static function exists( int $cid) : bool;
public static function yield();

/**
 * Suspends the coroutine.
 * Can be called only from within a coroutine.
 */
public static function suspend() : bool;

/** 
 * Resumes a suspended coroutine.
 * Can be called only on suspended coroutine.
 * The provided $cid must be of a suspended coroutine.
 * @param int $cid
 * @return bool
 */
public static function resume( int $cid) : bool;

/**
 * Returns an array with vairous data:
 * Array
 * (
 *     [event_num] => 0
 *     [signal_listener_num] => 0
 *     [aio_task_num] => 0
 *     [c_stack_size] => 2097152
 *     [coroutine_num] => 0
 *     [coroutine_peak_num] => 1
 *     [coroutine_last_cid] => 1
 * )
 *
 */
public static function stats();

/**
 * Returns the coroutine ID of the coroutine in which this method is called.
 * If called outside a coroutine returns -1
 * @return int
 */
public static function getCid() : int;

public static function getuid();

/**
 * Returns the parent coroutine ID of the current coroutine.
 * If there is no parent coroutine ID reurns -1
 * @return int
 */
public static function getPcid(int $cid) : int;

/**
 * Delays the execution of the current coroutine with the given amount in $seconds.
 * Does not block the worker (the other coroutines can execute).
 * @param int $seconds
 * @return void
 */
public static function sleep( $seconds) : void;

public static function fread( $handle,  $length);
public static function fgets( $handle);
public static function fwrite( $handle,  $string,  $length);
public static function readFile( $filename);
public static function writeFile( $filename,  $data,  $flags);
public static function getaddrinfo( $hostname,  $family,  $socktype,  $protocol,  $service);
public static function statvfs( $path);

/**
 * Returns an array like debug_backtrace() but for the coroutine only.
 * Invoking debug_backtrace() in a coroutine will produce nothing.
 * co::getBackTrace() is to be used within a coroutine or if used outside (or in another coroutine) the coroutine $cid must be provided.
 * Invkoing getBackTrace() with $cid for another coroutine is useful only if it is currently suspended
 * @param int $cid If invoked inside a coroutine is not required (0 can be provided and the cid of the current coroutine will be used)
 * @param int $options See debug_backtrace() $options argument
 * @param int $limit See debug_backtrace() $limit argument
 * @return array|bool
 */
public static function getBackTrace( int $cid,  $options, int $limit) : /* array|bool */ ;

/**
 * Get all the coroutines of current process.
 * Retruns a Swoole\Coroutine\Iterator holding the coroutine ID of all current coroutines.
 * NOTE: DOES NOT SEEM TO WORK - always returns an empty iterator
 * @return Swoole\Coroutine\Iterator
 */
public static function list() : Swoole\Coroutine\Iterator;

/**
 * Alias of self::list()
 */
public static function listCoroutines() : Swoole\Coroutine\Iterator;
```