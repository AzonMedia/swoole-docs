# Swoole\Constant

## Intrduction

## API

```php
<?php

namespace Swoole;

/**
 * Class Constant
 * @package Swoole
 */
class Constant
{
    
    /**
     * @var string
     */
    public const EVENT_RECEIVE = 'receive';
    
    /**
     * @var string
     */
    public const EVENT_CONNECT = 'connect';
    
    /**
     * @var string
     */
    public const EVENT_CLOSE = 'close';
    
    /**
     * @var string
     */
    public const EVENT_PACKET = 'packet';
    
    /**
     * @var string
     */
    public const EVENT_REQUEST = 'request';
    
    /**
     * @var string
     */
    public const EVENT_MESSAGE = 'message';
    
    /**
     * @var string
     */
    public const EVENT_OPEN = 'open';
    
    /**
     * @var string
     */
    public const EVENT_HANDSHAKE = 'handshake';
    
    /**
     * @var string
     */
    public const EVENT_TASK = 'task';
    
    /**
     * @var string
     */
    public const EVENT_FINISH = 'finish';
    
    /**
     * @var string
     */
    public const EVENT_START = 'start';
    
    /**
     * @var string
     */
    public const EVENT_SHUTDOWN = 'shutdown';
    
    /**
     * @var string
     */
    public const EVENT_WORKER_START = 'workerStart';
    
    /**
     * @var string
     */
    public const EVENT_WORKER_EXIT = 'workerExit';
    
    /**
     * @var string
     */
    public const EVENT_WORKER_ERROR = 'workerError';
    
    /**
     * @var string
     */
    public const EVENT_WORKER_STOP = 'workerStop';
    
    /**
     * @var string
     */
    public const EVENT_MANAGER_START = 'managerStart';
    
    /**
     * @var string
     */
    public const EVENT_MANAGER_STOP = 'managerStop';
    
    /**
     * @var string
     */
    public const EVENT_ERROR = 'error';
    
    /**
     * @var string
     */
    public const OPTION_ENABLE_SIGNALFD = 'enable_signalfd';
    
    /**
     * @var string
     */
    public const OPTION_DNS_CACHE_REFRESH_TIME = 'dns_cache_refresh_time';
    
    /**
     * @var string
     */
    public const OPTION_SOCKET_BUFFER_SIZE = 'socket_buffer_size';
    
    /**
     * @var string
     */
    public const OPTION_LOG_LEVEL = 'log_level';
    
    /**
     * @var string
     */
    public const OPTION_THREAD_NUM = 'thread_num';
    
    /**
     * @var string
     */
    public const OPTION_MIN_THREAD_NUM = 'min_thread_num';
    
    /**
     * @var string
     */
    public const OPTION_MAX_THREAD_NUM = 'max_thread_num';
    
    /**
     * @var string
     */
    public const OPTION_DISPLAY_ERRORS = 'display_errors';
    
    /**
     * @var string
     */
    public const OPTION_SOCKET_DONTWAIT = 'socket_dontwait';
    
    /**
     * @var string
     */
    public const OPTION_DNS_LOOKUP_RANDOM = 'dns_lookup_random';
    
    /**
     * @var string
     */
    public const OPTION_DNS_SERVER = 'dns_server';
    
    /**
     * @var string
     */
    public const OPTION_USE_ASYNC_RESOLVER = 'use_async_resolver';
    
    /**
     * @var string
     */
    public const OPTION_ENABLE_COROUTINE = 'enable_coroutine';
    
    /**
     * @var string
     */
    public const OPTION_ENABLE_REUSE_PORT = 'enable_reuse_port';
    
    /**
     * @var string
     */
    public const OPTION_SSL_METHOD = 'ssl_method';
    
    /**
     * @var string
     */
    public const OPTION_SSL_COMPRESS = 'ssl_compress';
    
    /**
     * @var string
     */
    public const OPTION_SSL_CERT_FILE = 'ssl_cert_file';
    
    /**
     * @var string
     */
    public const OPTION_SSL_KEY_FILE = 'ssl_key_file';
    
    /**
     * @var string
     */
    public const OPTION_SSL_PASSPHRASE = 'ssl_passphrase';
    
    /**
     * @var string
     */
    public const OPTION_SSL_HOST_NAME = 'ssl_host_name';
    
    /**
     * @var string
     */
    public const OPTION_SSL_VERIFY_PEER = 'ssl_verify_peer';
    
    /**
     * @var string
     */
    public const OPTION_SSL_ALLOW_SELF_SIGNED = 'ssl_allow_self_signed';
    
    /**
     * @var string
     */
    public const OPTION_SSL_CAFILE = 'ssl_cafile';
    
    /**
     * @var string
     */
    public const OPTION_SSL_CAPATH = 'ssl_capath';
    
    /**
     * @var string
     */
    public const OPTION_SSL_VERIFY_DEPTH = 'ssl_verify_depth';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_EOF_CHECK = 'open_eof_check';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_EOF_SPLIT = 'open_eof_split';
    
    /**
     * @var string
     */
    public const OPTION_PACKAGE_EOF = 'package_eof';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_MQTT_PROTOCOL = 'open_mqtt_protocol';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_LENGTH_CHECK = 'open_length_check';
    
    /**
     * @var string
     */
    public const OPTION_PACKAGE_LENGTH_TYPE = 'package_length_type';
    
    /**
     * @var string
     */
    public const OPTION_PACKAGE_LENGTH_OFFSET = 'package_length_offset';
    
    /**
     * @var string
     */
    public const OPTION_PACKAGE_BODY_OFFSET = 'package_body_offset';
    
    /**
     * @var string
     */
    public const OPTION_PACKAGE_LENGTH_FUNC = 'package_length_func';
    
    /**
     * @var string
     */
    public const OPTION_PACKAGE_MAX_LENGTH = 'package_max_length';
    
    /**
     * @var string
     */
    public const OPTION_BUFFER_HIGH_WATERMARK = 'buffer_high_watermark';
    
    /**
     * @var string
     */
    public const OPTION_BUFFER_LOW_WATERMARK = 'buffer_low_watermark';
    
    /**
     * @var string
     */
    public const OPTION_BIND_PORT = 'bind_port';
    
    /**
     * @var string
     */
    public const OPTION_BIND_ADDRESS = 'bind_address';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_TCP_NODELAY = 'open_tcp_nodelay';
    
    /**
     * @var string
     */
    public const OPTION_SOCKS5_HOST = 'socks5_host';
    
    /**
     * @var string
     */
    public const OPTION_SOCKS5_PORT = 'socks5_port';
    
    /**
     * @var string
     */
    public const OPTION_SOCKS5_USERNAME = 'socks5_username';
    
    /**
     * @var string
     */
    public const OPTION_SOCKS5_PASSWORD = 'socks5_password';
    
    /**
     * @var string
     */
    public const OPTION_HTTP_PROXY_HOST = 'http_proxy_host';
    
    /**
     * @var string
     */
    public const OPTION_HTTP_PROXY_PORT = 'http_proxy_port';
    
    /**
     * @var string
     */
    public const OPTION_HTTP_PROXY_USERNAME = 'http_proxy_username';
    
    /**
     * @var string
     */
    public const OPTION_HTTP_PROXY_USER = 'http_proxy_user';
    
    /**
     * @var string
     */
    public const OPTION_HTTP_PROXY_PASSWORD = 'http_proxy_password';
    
    /**
     * @var string
     */
    public const OPTION_TIMEOUT = 'timeout';
    
    /**
     * @var string
     */
    public const OPTION_CONNECT_TIMEOUT = 'connect_timeout';
    
    /**
     * @var string
     */
    public const OPTION_READ_TIMEOUT = 'read_timeout';
    
    /**
     * @var string
     */
    public const OPTION_WRITE_TIMEOUT = 'write_timeout';
    
    /**
     * @var string
     */
    public const OPTION_SSL_DISABLE_COMPRESSION = 'ssl_disable_compression';
    
    /**
     * @var string
     */
    public const OPTION_MAX_COROUTINE = 'max_coroutine';
    
    /**
     * @var string
     */
    public const OPTION_HOOK_FLAGS = 'hook_flags';
    
    /**
     * @var string
     */
    public const OPTION_C_STACK_SIZE = 'c_stack_size';
    
    /**
     * @var string
     */
    public const OPTION_STACK_SIZE = 'stack_size';
    
    /**
     * @var string
     */
    public const OPTION_SOCKET_CONNECT_TIMEOUT = 'socket_connect_timeout';
    
    /**
     * @var string
     */
    public const OPTION_SOCKET_TIMEOUT = 'socket_timeout';
    
    /**
     * @var string
     */
    public const OPTION_SOCKET_READ_TIMEOUT = 'socket_read_timeout';
    
    /**
     * @var string
     */
    public const OPTION_SOCKET_WRITE_TIMEOUT = 'socket_write_timeout';
    
    /**
     * @var string
     */
    public const OPTION_TRACE_FLAGS = 'trace_flags';
    
    /**
     * @var string
     */
    public const OPTION_DNS_CACHE_EXPIRE = 'dns_cache_expire';
    
    /**
     * @var string
     */
    public const OPTION_DNS_CACHE_CAPACITY = 'dns_cache_capacity';
    
    /**
     * @var string
     */
    public const OPTION_AIO_CORE_WORKER_NUM = 'aio_core_worker_num';
    
    /**
     * @var string
     */
    public const OPTION_AIO_WORKER_NUM = 'aio_worker_num';
    
    /**
     * @var string
     */
    public const OPTION_AIO_MAX_WAIT_TIME = 'aio_max_wait_time';
    
    /**
     * @var string
     */
    public const OPTION_AIO_MAX_IDLE_TIME = 'aio_max_idle_time';
    
    /**
     * @var string
     */
    public const OPTION_RECONNECT = 'reconnect';
    
    /**
     * @var string
     */
    public const OPTION_DEFER = 'defer';
    
    /**
     * @var string
     */
    public const OPTION_KEEP_ALIVE = 'keep_alive';
    
    /**
     * @var string
     */
    public const OPTION_WEBSOCKET_MASK = 'websocket_mask';
    
    /**
     * @var string
     */
    public const OPTION_HOST = 'host';
    
    /**
     * @var string
     */
    public const OPTION_PORT = 'port';
    
    /**
     * @var string
     */
    public const OPTION_SSL = 'ssl';
    
    /**
     * @var string
     */
    public const OPTION_USER = 'user';
    
    /**
     * @var string
     */
    public const OPTION_PASSWORD = 'password';
    
    /**
     * @var string
     */
    public const OPTION_DATABASE = 'database';
    
    /**
     * @var string
     */
    public const OPTION_CHARSET = 'charset';
    
    /**
     * @var string
     */
    public const OPTION_STRICT_TYPE = 'strict_type';
    
    /**
     * @var string
     */
    public const OPTION_FETCH_MODE = 'fetch_mode';
    
    /**
     * @var string
     */
    public const OPTION_SERIALIZE = 'serialize';
    
    /**
     * @var string
     */
    public const OPTION_COMPATIBILITY_MODE = 'compatibility_mode';
    
    /**
     * @var string
     */
    public const OPTION_CHROOT = 'chroot';
    
    /**
     * @var string
     */
    public const OPTION_GROUP = 'group';
    
    /**
     * @var string
     */
    public const OPTION_DAEMONIZE = 'daemonize';
    
    /**
     * @var string
     */
    public const OPTION_DEBUG_MODE = 'debug_mode';
    
    /**
     * @var string
     */
    public const OPTION_PID_FILE = 'pid_file';
    
    /**
     * @var string
     */
    public const OPTION_REACTOR_NUM = 'reactor_num';
    
    /**
     * @var string
     */
    public const OPTION_SINGLE_THREAD = 'single_thread';
    
    /**
     * @var string
     */
    public const OPTION_WORKER_NUM = 'worker_num';
    
    /**
     * @var string
     */
    public const OPTION_MAX_WAIT_TIME = 'max_wait_time';
    
    /**
     * @var string
     */
    public const OPTION_MAX_CORO_NUM = 'max_coro_num';
    
    /**
     * @var string
     */
    public const OPTION_SEND_YIELD = 'send_yield';
    
    /**
     * @var string
     */
    public const OPTION_SEND_TIMEOUT = 'send_timeout';
    
    /**
     * @var string
     */
    public const OPTION_DISPATCH_MODE = 'dispatch_mode';
    
    /**
     * @var string
     */
    public const OPTION_DISPATCH_FUNC = 'dispatch_func';
    
    /**
     * @var string
     */
    public const OPTION_LOG_FILE = 'log_file';
    
    /**
     * @var string
     */
    public const OPTION_DISCARD_TIMEOUT_REQUEST = 'discard_timeout_request';
    
    /**
     * @var string
     */
    public const OPTION_ENABLE_UNSAFE_EVENT = 'enable_unsafe_event';
    
    /**
     * @var string
     */
    public const OPTION_ENABLE_DELAY_RECEIVE = 'enable_delay_receive';
    
    /**
     * @var string
     */
    public const OPTION_TASK_USE_OBJECT = 'task_use_object';
    
    /**
     * @var string
     */
    public const OPTION_TASK_ENABLE_COROUTINE = 'task_enable_coroutine';
    
    /**
     * @var string
     */
    public const OPTION_TASK_WORKER_NUM = 'task_worker_num';
    
    /**
     * @var string
     */
    public const OPTION_TRACE_EVENT_WORKER = 'trace_event_worker';
    
    /**
     * @var string
     */
    public const OPTION_REQUEST_SLOWLOG_TIMEOUT = 'request_slowlog_timeout';
    
    /**
     * @var string
     */
    public const OPTION_REQUEST_SLOWLOG_FILE = 'request_slowlog_file';
    
    /**
     * @var string
     */
    public const OPTION_TASK_IPC_MODE = 'task_ipc_mode';
    
    /**
     * @var string
     */
    public const OPTION_TASK_TMPDIR = 'task_tmpdir';
    
    /**
     * @var string
     */
    public const OPTION_TASK_MAX_REQUEST = 'task_max_request';
    
    /**
     * @var string
     */
    public const OPTION_MAX_CONNECTION = 'max_connection';
    
    /**
     * @var string
     */
    public const OPTION_MAX_CONN = 'max_conn';
    
    /**
     * @var string
     */
    public const OPTION_HEARTBEAT_CHECK_INTERVAL = 'heartbeat_check_interval';
    
    /**
     * @var string
     */
    public const OPTION_HEARTBEAT_IDLE_TIME = 'heartbeat_idle_time';
    
    /**
     * @var string
     */
    public const OPTION_MAX_REQUEST = 'max_request';
    
    /**
     * @var string
     */
    public const OPTION_RELOAD_ASYNC = 'reload_async';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_CPU_AFFINITY = 'open_cpu_affinity';
    
    /**
     * @var string
     */
    public const OPTION_CPU_AFFINITY_IGNORE = 'cpu_affinity_ignore';
    
    /**
     * @var string
     */
    public const OPTION_HTTP_PARSE_COOKIE = 'http_parse_cookie';
    
    /**
     * @var string
     */
    public const OPTION_HTTP_PARSE_POST = 'http_parse_post';
    
    /**
     * @var string
     */
    public const OPTION_HTTP_PARSE_FILES = 'http_parse_files';
    
    /**
     * @var string
     */
    public const OPTION_HTTP_COMPRESSION = 'http_compression';
    
    /**
     * @var string
     */
    public const OPTION_HTTP_GZIP_LEVEL = 'http_gzip_level';
    
    /**
     * @var string
     */
    public const OPTION_HTTP_COMPRESSION_LEVEL = 'http_compression_level';
    
    /**
     * @var string
     */
    public const OPTION_UPLOAD_TMP_DIR = 'upload_tmp_dir';
    
    /**
     * @var string
     */
    public const OPTION_ENABLE_STATIC_HANDLER = 'enable_static_handler';
    
    /**
     * @var string
     */
    public const OPTION_DOCUMENT_ROOT = 'document_root';
    
    /**
     * @var string
     */
    public const OPTION_STATIC_HANDLER_LOCATIONS = 'static_handler_locations';
    
    /**
     * @var string
     */
    public const OPTION_BUFFER_INPUT_SIZE = 'buffer_input_size';
    
    /**
     * @var string
     */
    public const OPTION_BUFFER_OUTPUT_SIZE = 'buffer_output_size';
    
    /**
     * @var string
     */
    public const OPTION_MESSAGE_QUEUE_KEY = 'message_queue_key';
    
    /**
     * @var string
     */
    public const OPTION_BACKLOG = 'backlog';
    
    /**
     * @var string
     */
    public const OPTION_KERNEL_SOCKET_RECV_BUFFER_SIZE = 'kernel_socket_recv_buffer_size';
    
    /**
     * @var string
     */
    public const OPTION_KERNEL_SOCKET_SEND_BUFFER_SIZE = 'kernel_socket_send_buffer_size';
    
    /**
     * @var string
     */
    public const OPTION_TCP_DEFER_ACCEPT = 'tcp_defer_accept';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_TCP_KEEPALIVE = 'open_tcp_keepalive';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_HTTP_PROTOCOL = 'open_http_protocol';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_WEBSOCKET_PROTOCOL = 'open_websocket_protocol';
    
    /**
     * @var string
     */
    public const OPTION_WEBSOCKET_SUBPROTOCOL = 'websocket_subprotocol';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_WEBSOCKET_CLOSE_FRAME = 'open_websocket_close_frame';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_HTTP2_PROTOCOL = 'open_http2_protocol';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_REDIS_PROTOCOL = 'open_redis_protocol';
    
    /**
     * @var string
     */
    public const OPTION_TCP_KEEPIDLE = 'tcp_keepidle';
    
    /**
     * @var string
     */
    public const OPTION_TCP_KEEPINTERVAL = 'tcp_keepinterval';
    
    /**
     * @var string
     */
    public const OPTION_TCP_KEEPCOUNT = 'tcp_keepcount';
    
    /**
     * @var string
     */
    public const OPTION_TCP_FASTOPEN = 'tcp_fastopen';
    
    /**
     * @var string
     */
    public const OPTION_PACKAGE_BODY_START = 'package_body_start';
    
    /**
     * @var string
     */
    public const OPTION_SSL_CLIENT_CERT_FILE = 'ssl_client_cert_file';
    
    /**
     * @var string
     */
    public const OPTION_SSL_PREFER_SERVER_CIPHERS = 'ssl_prefer_server_ciphers';
    
    /**
     * @var string
     */
    public const OPTION_SSL_CIPHERS = 'ssl_ciphers';
    
    /**
     * @var string
     */
    public const OPTION_SSL_ECDH_CURVE = 'ssl_ecdh_curve';
    
    /**
     * @var string
     */
    public const OPTION_SSL_DHPARAM = 'ssl_dhparam';
    
    /**
     * @var string
     */
    public const OPTION_OPEN_SSL = 'open_ssl';
    
    
}


```

## Examples

