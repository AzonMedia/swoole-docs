# Swoole\Coroutine\Redis

## Intrduction

## API

```php
<?php

namespace Swoole\Coroutine;

/**
 * Class Redis
 * @package Swoole\Coroutine
 */
class Redis
{
    /**
     * @var 
     */
    public $host;
    
    /**
     * @var 
     */
    public $port;
    
    /**
     * @var 
     */
    public $setting;
    
    /**
     * @var integer
     */
    public $sock = -1;
    
    /**
     * @var 
     */
    public $connected;
    
    /**
     * @var 
     */
    public $errType;
    
    /**
     * @var 
     */
    public $errCode;
    
    /**
     * @var 
     */
    public $errMsg;
    
    
    
    /**
     * @param type $config
     * @return void
     */
    public function __construct( $config) { }
    
    /**
     * 
     * @return void
     */
    public function __destruct( ) { }
    
    /**
     * @param type $host
     * @param type $port
     * @param type $serialize
     * @return void
     */
    public function connect( $host, $port, $serialize) { }
    
    /**
     * 
     * @return void
     */
    public function getAuth( ) { }
    
    /**
     * 
     * @return void
     */
    public function getDBNum( ) { }
    
    /**
     * 
     * @return void
     */
    public function getOptions( ) { }
    
    /**
     * @param type $options
     * @return void
     */
    public function setOptions( $options) { }
    
    /**
     * 
     * @return void
     */
    public function getDefer( ) { }
    
    /**
     * @param type $defer
     * @return void
     */
    public function setDefer( $defer) { }
    
    /**
     * 
     * @return void
     */
    public function recv( ) { }
    
    /**
     * @param array $params
     * @return void
     */
    public function request( array $params) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) { }
    
    /**
     * @param type $key
     * @param type $value
     * @param type $timeout
     * @param type $opt
     * @return void
     */
    public function set( $key, $value, $timeout, $opt) { }
    
    /**
     * @param type $key
     * @param type $offset
     * @param type $value
     * @return void
     */
    public function setBit( $key, $offset, $value) { }
    
    /**
     * @param type $key
     * @param type $expire
     * @param type $value
     * @return void
     */
    public function setEx( $key, $expire, $value) { }
    
    /**
     * @param type $key
     * @param type $expire
     * @param type $value
     * @return void
     */
    public function psetEx( $key, $expire, $value) { }
    
    /**
     * @param type $key
     * @param type $index
     * @param type $value
     * @return void
     */
    public function lSet( $key, $index, $value) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function get( $key) { }
    
    /**
     * @param type $keys
     * @return void
     */
    public function mGet( $keys) { }
    
    /**
     * @param type $key
     * @param type $other_keys
     * @return void
     */
    public function del( $key, $other_keys) { }
    
    /**
     * @param type $key
     * @param type $member
     * @param type $other_members
     * @return void
     */
    public function hDel( $key, $member, $other_members) { }
    
    /**
     * @param type $key
     * @param type $member
     * @param type $value
     * @return void
     */
    public function hSet( $key, $member, $value) { }
    
    /**
     * @param type $key
     * @param type $pairs
     * @return void
     */
    public function hMSet( $key, $pairs) { }
    
    /**
     * @param type $key
     * @param type $member
     * @param type $value
     * @return void
     */
    public function hSetNx( $key, $member, $value) { }
    
    /**
     * @param type $key
     * @param type $other_keys
     * @return void
     */
    public function delete( $key, $other_keys) { }
    
    /**
     * @param type $pairs
     * @return void
     */
    public function mSet( $pairs) { }
    
    /**
     * @param type $pairs
     * @return void
     */
    public function mSetNx( $pairs) { }
    
    /**
     * @param type $pattern
     * @return void
     */
    public function getKeys( $pattern) { }
    
    /**
     * @param type $pattern
     * @return void
     */
    public function keys( $pattern) { }
    
    /**
     * @param type $key
     * @param type $other_keys
     * @return void
     */
    public function exists( $key, $other_keys) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function type( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function strLen( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function lPop( $key) { }
    
    /**
     * @param type $key
     * @param type $timeout_or_key
     * @param type $extra_args
     * @return void
     */
    public function blPop( $key, $timeout_or_key, $extra_args) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function rPop( $key) { }
    
    /**
     * @param type $key
     * @param type $timeout_or_key
     * @param type $extra_args
     * @return void
     */
    public function brPop( $key, $timeout_or_key, $extra_args) { }
    
    /**
     * @param type $src
     * @param type $dst
     * @param type $timeout
     * @return void
     */
    public function bRPopLPush( $src, $dst, $timeout) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function lSize( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function lLen( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function sSize( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function scard( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function sPop( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function sMembers( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function sGetMembers( $key) { }
    
    /**
     * @param type $key
     * @param type $count
     * @return void
     */
    public function sRandMember( $key, $count) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function persist( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function ttl( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function pttl( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function zCard( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function zSize( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function hLen( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function hKeys( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function hVals( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function hGetAll( $key) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function debug( $key) { }
    
    /**
     * @param type $ttl
     * @param type $key
     * @param type $value
     * @return void
     */
    public function restore( $ttl, $key, $value) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function dump( $key) { }
    
    /**
     * @param type $key
     * @param type $newkey
     * @return void
     */
    public function renameKey( $key, $newkey) { }
    
    /**
     * @param type $key
     * @param type $newkey
     * @return void
     */
    public function rename( $key, $newkey) { }
    
    /**
     * @param type $key
     * @param type $newkey
     * @return void
     */
    public function renameNx( $key, $newkey) { }
    
    /**
     * @param type $src
     * @param type $dst
     * @return void
     */
    public function rpoplpush( $src, $dst) { }
    
    /**
     * 
     * @return void
     */
    public function randomKey( ) { }
    
    /**
     * @param type $key
     * @param type $elements
     * @return void
     */
    public function pfadd( $key, $elements) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function pfcount( $key) { }
    
    /**
     * @param type $dstkey
     * @param type $keys
     * @return void
     */
    public function pfmerge( $dstkey, $keys) { }
    
    /**
     * 
     * @return void
     */
    public function ping( ) { }
    
    /**
     * @param type $password
     * @return void
     */
    public function auth( $password) { }
    
    /**
     * 
     * @return void
     */
    public function unwatch( ) { }
    
    /**
     * @param type $key
     * @param type $other_keys
     * @return void
     */
    public function watch( $key, $other_keys) { }
    
    /**
     * 
     * @return void
     */
    public function save( ) { }
    
    /**
     * 
     * @return void
     */
    public function bgSave( ) { }
    
    /**
     * 
     * @return void
     */
    public function lastSave( ) { }
    
    /**
     * 
     * @return void
     */
    public function flushDB( ) { }
    
    /**
     * 
     * @return void
     */
    public function flushAll( ) { }
    
    /**
     * 
     * @return void
     */
    public function dbSize( ) { }
    
    /**
     * 
     * @return void
     */
    public function bgrewriteaof( ) { }
    
    /**
     * 
     * @return void
     */
    public function time( ) { }
    
    /**
     * 
     * @return void
     */
    public function role( ) { }
    
    /**
     * @param type $key
     * @param type $offset
     * @param type $value
     * @return void
     */
    public function setRange( $key, $offset, $value) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function setNx( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function getSet( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function append( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function lPushx( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function lPush( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function rPush( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function rPushx( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function sContains( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function sismember( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $member
     * @return void
     */
    public function zScore( $key, $member) { }
    
    /**
     * @param type $key
     * @param type $member
     * @return void
     */
    public function zRank( $key, $member) { }
    
    /**
     * @param type $key
     * @param type $member
     * @return void
     */
    public function zRevRank( $key, $member) { }
    
    /**
     * @param type $key
     * @param type $member
     * @return void
     */
    public function hGet( $key, $member) { }
    
    /**
     * @param type $key
     * @param type $keys
     * @return void
     */
    public function hMGet( $key, $keys) { }
    
    /**
     * @param type $key
     * @param type $member
     * @return void
     */
    public function hExists( $key, $member) { }
    
    /**
     * @param type $channel
     * @param type $message
     * @return void
     */
    public function publish( $channel, $message) { }
    
    /**
     * @param type $key
     * @param type $value
     * @param type $member
     * @return void
     */
    public function zIncrBy( $key, $value, $member) { }
    
    /**
     * @param type $key
     * @param type $score
     * @param type $value
     * @return void
     */
    public function zAdd( $key, $score, $value) { }
    
    /**
     * @param type $key
     * @param type $min
     * @param type $max
     * @return void
     */
    public function zDeleteRangeByScore( $key, $min, $max) { }
    
    /**
     * @param type $key
     * @param type $min
     * @param type $max
     * @return void
     */
    public function zRemRangeByScore( $key, $min, $max) { }
    
    /**
     * @param type $key
     * @param type $min
     * @param type $max
     * @return void
     */
    public function zCount( $key, $min, $max) { }
    
    /**
     * @param type $key
     * @param type $start
     * @param type $end
     * @param type $scores
     * @return void
     */
    public function zRange( $key, $start, $end, $scores) { }
    
    /**
     * @param type $key
     * @param type $start
     * @param type $end
     * @param type $scores
     * @return void
     */
    public function zRevRange( $key, $start, $end, $scores) { }
    
    /**
     * @param type $key
     * @param type $start
     * @param type $end
     * @param type $options
     * @return void
     */
    public function zRangeByScore( $key, $start, $end, $options) { }
    
    /**
     * @param type $key
     * @param type $start
     * @param type $end
     * @param type $options
     * @return void
     */
    public function zRevRangeByScore( $key, $start, $end, $options) { }
    
    /**
     * @param type $key
     * @param type $min
     * @param type $max
     * @param type $offset
     * @param type $limit
     * @return void
     */
    public function zRangeByLex( $key, $min, $max, $offset, $limit) { }
    
    /**
     * @param type $key
     * @param type $min
     * @param type $max
     * @param type $offset
     * @param type $limit
     * @return void
     */
    public function zRevRangeByLex( $key, $min, $max, $offset, $limit) { }
    
    /**
     * @param type $key
     * @param type $keys
     * @param type $weights
     * @param type $aggregate
     * @return void
     */
    public function zInter( $key, $keys, $weights, $aggregate) { }
    
    /**
     * @param type $key
     * @param type $keys
     * @param type $weights
     * @param type $aggregate
     * @return void
     */
    public function zinterstore( $key, $keys, $weights, $aggregate) { }
    
    /**
     * @param type $key
     * @param type $keys
     * @param type $weights
     * @param type $aggregate
     * @return void
     */
    public function zUnion( $key, $keys, $weights, $aggregate) { }
    
    /**
     * @param type $key
     * @param type $keys
     * @param type $weights
     * @param type $aggregate
     * @return void
     */
    public function zunionstore( $key, $keys, $weights, $aggregate) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function incrBy( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $member
     * @param type $value
     * @return void
     */
    public function hIncrBy( $key, $member, $value) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function incr( $key) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function decrBy( $key, $value) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function decr( $key) { }
    
    /**
     * @param type $key
     * @param type $offset
     * @return void
     */
    public function getBit( $key, $offset) { }
    
    /**
     * @param type $key
     * @param type $position
     * @param type $pivot
     * @param type $value
     * @return void
     */
    public function lInsert( $key, $position, $pivot, $value) { }
    
    /**
     * @param type $key
     * @param type $index
     * @return void
     */
    public function lGet( $key, $index) { }
    
    /**
     * @param type $key
     * @param type $integer
     * @return void
     */
    public function lIndex( $key, $integer) { }
    
    /**
     * @param type $key
     * @param type $timeout
     * @return void
     */
    public function setTimeout( $key, $timeout) { }
    
    /**
     * @param type $key
     * @param type $integer
     * @return void
     */
    public function expire( $key, $integer) { }
    
    /**
     * @param type $key
     * @param type $timestamp
     * @return void
     */
    public function pexpire( $key, $timestamp) { }
    
    /**
     * @param type $key
     * @param type $timestamp
     * @return void
     */
    public function expireAt( $key, $timestamp) { }
    
    /**
     * @param type $key
     * @param type $timestamp
     * @return void
     */
    public function pexpireAt( $key, $timestamp) { }
    
    /**
     * @param type $key
     * @param type $dbindex
     * @return void
     */
    public function move( $key, $dbindex) { }
    
    /**
     * @param type $dbindex
     * @return void
     */
    public function select( $dbindex) { }
    
    /**
     * @param type $key
     * @param type $start
     * @param type $end
     * @return void
     */
    public function getRange( $key, $start, $end) { }
    
    /**
     * @param type $key
     * @param type $start
     * @param type $stop
     * @return void
     */
    public function listTrim( $key, $start, $stop) { }
    
    /**
     * @param type $key
     * @param type $start
     * @param type $stop
     * @return void
     */
    public function ltrim( $key, $start, $stop) { }
    
    /**
     * @param type $key
     * @param type $start
     * @param type $end
     * @return void
     */
    public function lGetRange( $key, $start, $end) { }
    
    /**
     * @param type $key
     * @param type $start
     * @param type $end
     * @return void
     */
    public function lRange( $key, $start, $end) { }
    
    /**
     * @param type $key
     * @param type $value
     * @param type $count
     * @return void
     */
    public function lRem( $key, $value, $count) { }
    
    /**
     * @param type $key
     * @param type $value
     * @param type $count
     * @return void
     */
    public function lRemove( $key, $value, $count) { }
    
    /**
     * @param type $key
     * @param type $start
     * @param type $end
     * @return void
     */
    public function zDeleteRangeByRank( $key, $start, $end) { }
    
    /**
     * @param type $key
     * @param type $min
     * @param type $max
     * @return void
     */
    public function zRemRangeByRank( $key, $min, $max) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function incrByFloat( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $member
     * @param type $value
     * @return void
     */
    public function hIncrByFloat( $key, $member, $value) { }
    
    /**
     * @param type $key
     * @return void
     */
    public function bitCount( $key) { }
    
    /**
     * @param type $operation
     * @param type $ret_key
     * @param type $key
     * @param type $other_keys
     * @return void
     */
    public function bitOp( $operation, $ret_key, $key, $other_keys) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function sAdd( $key, $value) { }
    
    /**
     * @param type $src
     * @param type $dst
     * @param type $value
     * @return void
     */
    public function sMove( $src, $dst, $value) { }
    
    /**
     * @param type $key
     * @param type $other_keys
     * @return void
     */
    public function sDiff( $key, $other_keys) { }
    
    /**
     * @param type $dst
     * @param type $key
     * @param type $other_keys
     * @return void
     */
    public function sDiffStore( $dst, $key, $other_keys) { }
    
    /**
     * @param type $key
     * @param type $other_keys
     * @return void
     */
    public function sUnion( $key, $other_keys) { }
    
    /**
     * @param type $dst
     * @param type $key
     * @param type $other_keys
     * @return void
     */
    public function sUnionStore( $dst, $key, $other_keys) { }
    
    /**
     * @param type $key
     * @param type $other_keys
     * @return void
     */
    public function sInter( $key, $other_keys) { }
    
    /**
     * @param type $dst
     * @param type $key
     * @param type $other_keys
     * @return void
     */
    public function sInterStore( $dst, $key, $other_keys) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function sRemove( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $value
     * @return void
     */
    public function srem( $key, $value) { }
    
    /**
     * @param type $key
     * @param type $member
     * @param type $other_members
     * @return void
     */
    public function zDelete( $key, $member, $other_members) { }
    
    /**
     * @param type $key
     * @param type $member
     * @param type $other_members
     * @return void
     */
    public function zRemove( $key, $member, $other_members) { }
    
    /**
     * @param type $key
     * @param type $member
     * @param type $other_members
     * @return void
     */
    public function zRem( $key, $member, $other_members) { }
    
    /**
     * @param type $patterns
     * @return void
     */
    public function pSubscribe( $patterns) { }
    
    /**
     * @param type $channels
     * @return void
     */
    public function subscribe( $channels) { }
    
    /**
     * @param type $channels
     * @return void
     */
    public function unsubscribe( $channels) { }
    
    /**
     * @param type $patterns
     * @return void
     */
    public function pUnSubscribe( $patterns) { }
    
    /**
     * 
     * @return void
     */
    public function multi( ) { }
    
    /**
     * 
     * @return void
     */
    public function exec( ) { }
    
    /**
     * @param type $script
     * @param type $args
     * @param type $num_keys
     * @return void
     */
    public function eval( $script, $args, $num_keys) { }
    
    /**
     * @param type $script_sha
     * @param type $args
     * @param type $num_keys
     * @return void
     */
    public function evalSha( $script_sha, $args, $num_keys) { }
    
    /**
     * @param type $cmd
     * @param type $args
     * @return void
     */
    public function script( $cmd, $args) { }
    
}


```

## Examples

