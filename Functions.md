# Swoole Functions

## Introduction

## API

#### Global Functions

```php
<?php

/**
 * 
 * @return void
 */
function swoole_version( ) { }

/**
 * 
 * @return void
 */
function swoole_cpu_num( ) { }

/**
 * 
 * @return void
 */
function swoole_last_error( ) { }

/**
 * @param type $domain_name
 * @param type $timeout
 * @return void
 */
function swoole_async_dns_lookup_coro( $domain_name, $timeout) { }

/**
 * @param array $settings
 * @return void
 */
function swoole_async_set( array $settings) { }

/**
 * @param callable $func
 * @param ...$params
 * @return void
 */
function swoole_coroutine_create( callable $func, $params) { }

/**
 * @param callable $callback
 * @return void
 */
function swoole_coroutine_defer( callable $callback) { }

/**
 * @param &type $read_array
 * @param &type $write_array
 * @param &type $error_array
 * @param type $timeout
 * @return void
 */
function swoole_client_select( &$read_array, &$write_array, &$error_array, $timeout) { }

/**
 * @param &type $read_array
 * @param &type $write_array
 * @param &type $error_array
 * @param type $timeout
 * @return void
 */
function swoole_select( &$read_array, &$write_array, &$error_array, $timeout) { }

/**
 * @param type $process_name
 * @return void
 */
function swoole_set_process_name( $process_name) { }

/**
 * 
 * @return void
 */
function swoole_get_local_ip( ) { }

/**
 * 
 * @return void
 */
function swoole_get_local_mac( ) { }

/**
 * @param type $errno
 * @param type $error_type
 * @return void
 */
function swoole_strerror( $errno, $error_type) { }

/**
 * 
 * @return void
 */
function swoole_errno( ) { }

/**
 * @param type $data
 * @param type $type
 * @return void
 */
function swoole_hashcode( $data, $type) { }

/**
 * @param type $filename
 * @return void
 */
function swoole_get_mime_type( $filename) { }

/**
 * 
 * @return void
 */
function swoole_clear_dns_cache( ) { }

/**
 * 
 * @return void
 */
function swoole_internal_call_user_shutdown_begin( ) { }

/**
 * @param type $fd
 * @param null|callable $read_callback
 * @param null|callable $write_callback
 * @param type $events
 * @return void
 */
function swoole_event_add( $fd, ?callable $read_callback, ?callable $write_callback, $events) { }

/**
 * @param type $fd
 * @return void
 */
function swoole_event_del( $fd) { }

/**
 * @param type $fd
 * @param null|callable $read_callback
 * @param null|callable $write_callback
 * @param type $events
 * @return void
 */
function swoole_event_set( $fd, ?callable $read_callback, ?callable $write_callback, $events) { }

/**
 * @param type $fd
 * @param type $events
 * @return void
 */
function swoole_event_isset( $fd, $events) { }

/**
 * 
 * @return void
 */
function swoole_event_dispatch( ) { }

/**
 * @param callable $callback
 * @return void
 */
function swoole_event_defer( callable $callback) { }

/**
 * @param null|callable $callback
 * @param type $before
 * @return void
 */
function swoole_event_cycle( ?callable $callback, $before) { }

/**
 * @param type $fd
 * @param type $data
 * @return void
 */
function swoole_event_write( $fd, $data) { }

/**
 * 
 * @return void
 */
function swoole_event_wait( ) { }

/**
 * 
 * @return void
 */
function swoole_event_exit( ) { }

/**
 * @param array $settings
 * @return void
 */
function swoole_timer_set( array $settings) { }

/**
 * @param type $ms
 * @param callable $callback
 * @return void
 */
function swoole_timer_after( $ms, callable $callback) { }

/**
 * @param type $ms
 * @param callable $callback
 * @return void
 */
function swoole_timer_tick( $ms, callable $callback) { }

/**
 * @param type $timer_id
 * @return void
 */
function swoole_timer_exists( $timer_id) { }

/**
 * @param type $timer_id
 * @return void
 */
function swoole_timer_info( $timer_id) { }

/**
 * 
 * @return void
 */
function swoole_timer_stats( ) { }

/**
 * 
 * @return void
 */
function swoole_timer_list( ) { }

/**
 * @param type $timer_id
 * @return void
 */
function swoole_timer_clear( $timer_id) { }

/**
 * 
 * @return void
 */
function swoole_timer_clear_all( ) { }

/**
 * @param string $command
 * @param &type $output
 * @param &type $returnVar
 * @return void
 */
function swoole_exec( string $command, &$output = NULL, &$returnVar = NULL) { }

/**
 * @param string $cmd
 * @return void
 */
function swoole_shell_exec( string $cmd) { }

/**
 * @param type $url
 * @return \Swoole\Curl\Handler
 */
function swoole_curl_init( $url = NULL) : \Swoole\Curl\Handler { }

/**
 * @param Swoole\Curl\Handler $obj
 * @param $opt
 * @param $value
 * @return bool
 * @throws Swoole\Curl\Exception
 */
function swoole_curl_setopt( \Swoole\Curl\Handler $obj, $opt, $value) : bool { }

/**
 * @param Swoole\Curl\Handler $obj
 * @param $array
 * @return bool
 * @throws Swoole\Curl\Exception
 */
function swoole_curl_setopt_array( \Swoole\Curl\Handler $obj, $array) : bool { }

/**
 * @param \Swoole\Curl\Handler $obj
 * @return void
 */
function swoole_curl_exec( \Swoole\Curl\Handler $obj) { }

/**
 * @param \Swoole\Curl\Handler $obj
 * @return null|string
 */
function swoole_curl_multi_getcontent( \Swoole\Curl\Handler $obj) : ?string { }

/**
 * @param \Swoole\Curl\Handler $obj
 * @return void
 */
function swoole_curl_close( \Swoole\Curl\Handler $obj) : void { }

/**
 * @param \Swoole\Curl\Handler $obj
 * @return string
 */
function swoole_curl_error( \Swoole\Curl\Handler $obj) : string { }

/**
 * @param \Swoole\Curl\Handler $obj
 * @return int
 */
function swoole_curl_errno( \Swoole\Curl\Handler $obj) : int { }

/**
 * @param \Swoole\Curl\Handler $obj
 * @return void
 */
function swoole_curl_reset( \Swoole\Curl\Handler $obj) : void { }

/**
 * @param \Swoole\Curl\Handler $obj
 * @param int $opt
 * @return void
 */
function swoole_curl_getinfo( \Swoole\Curl\Handler $obj, int $opt = 0) { }

/**
 * @param string $string
 * @return Swoole\StringObject
 */
function swoole_string( string $string = '') : \Swoole\StringObject { }

/**
 * @param array $array
 * @return Swoole\ArrayObject
 */
function swoole_array( array $array = array (
)) : \Swoole\ArrayObject { }

/**
 * @param array $array
 * @param $key
 * @param $default_value
 * @return mixed
 */
function swoole_array_default_value( array $array, $key, $default_value = '') { }

```

#### Namespaced functions

```php
<?php

namespace Swoole\Coroutine; 

/**
 * @param callable $fn
 * @param ...$args
 * @return void
 */
function run( callable $fn, $args) { }
```