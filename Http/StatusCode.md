# Swoole\Http\StatusCode

## Intrduction

## API

```php
<?php

namespace Swoole\Http;

/**
 * Class StatusCode
 * @package Swoole\Http
 */
abstract class StatusCode
{
    /**
     * @var array
     */
    protected static $reasonPhrases = array (
      100 => 'Continue',
      101 => 'Switching Protocols',
      102 => 'Processing',
      200 => 'OK',
      201 => 'Created',
      202 => 'Accepted',
      203 => 'Non-Authoritative Information',
      204 => 'No Content',
      205 => 'Reset Content',
      206 => 'Partial Content',
      207 => 'Multi-status',
      208 => 'Already Reported',
      226 => 'IM Used',
      300 => 'Multiple Choices',
      301 => 'Moved Permanently',
      302 => 'Found',
      303 => 'See Other',
      304 => 'Not Modified',
      305 => 'Use Proxy',
      306 => 'Switch Proxy',
      307 => 'Temporary Redirect',
      308 => 'Permanent Redirect',
      400 => 'Bad Request',
      401 => 'Unauthorized',
      402 => 'Payment Required',
      403 => 'Forbidden',
      404 => 'Not Found',
      405 => 'Method Not Allowed',
      406 => 'Not Acceptable',
      407 => 'Proxy Authentication Required',
      408 => 'Request Time-out',
      409 => 'Conflict',
      410 => 'Gone',
      411 => 'Length Required',
      412 => 'Precondition Failed',
      413 => 'Request Entity Too Large',
      414 => 'Request-URI Too Large',
      415 => 'Unsupported Media Type',
      416 => 'Requested range not satisfiable',
      417 => 'Expectation Failed',
      421 => 'Unprocessable Entity',
      422 => 'Unprocessable Entity',
      423 => 'Locked',
      424 => 'Failed Dependency',
      425 => 'Unordered Collection',
      426 => 'Upgrade Required',
      428 => 'Precondition Required',
      429 => 'Too Many Requests',
      431 => 'Request Header Fields Too Large',
      451 => 'Unavailable For Legal Reasons',
      500 => 'Internal Server Error',
      501 => 'Not Implemented',
      502 => 'Bad Gateway',
      503 => 'Service Unavailable',
      504 => 'Gateway Time-out',
      505 => 'HTTP Version not supported',
      506 => 'Variant Also Negotiates',
      507 => 'Insufficient Storage',
      508 => 'Loop Detected',
      510 => 'Not Extended',
      511 => 'Network Authentication Required',
    );
    
    
    /**
     * @var integer
     */
    public const CONTINUE = 100;
    
    /**
     * @var integer
     */
    public const SWITCHING_PROTOCOLS = 101;
    
    /**
     * @var integer
     */
    public const PROCESSING = 102;
    
    /**
     * @var integer
     */
    public const OK = 200;
    
    /**
     * @var integer
     */
    public const CREATED = 201;
    
    /**
     * @var integer
     */
    public const ACCEPTED = 202;
    
    /**
     * @var integer
     */
    public const NON_AUTHORITATIVE_INFORMATION = 203;
    
    /**
     * @var integer
     */
    public const NO_CONTENT = 204;
    
    /**
     * @var integer
     */
    public const RESET_CONTENT = 205;
    
    /**
     * @var integer
     */
    public const PARTIAL_CONTENT = 206;
    
    /**
     * @var integer
     */
    public const MULTI_STATUS = 207;
    
    /**
     * @var integer
     */
    public const ALREADY_REPORTED = 208;
    
    /**
     * @var integer
     */
    public const IM_USED = 226;
    
    /**
     * @var integer
     */
    public const MULTIPLE_CHOICES = 300;
    
    /**
     * @var integer
     */
    public const MOVED_PERMANENTLY = 301;
    
    /**
     * @var integer
     */
    public const FOUND = 302;
    
    /**
     * @var integer
     */
    public const SEE_OTHER = 303;
    
    /**
     * @var integer
     */
    public const NOT_MODIFIED = 304;
    
    /**
     * @var integer
     */
    public const USE_PROXY = 305;
    
    /**
     * @var integer
     */
    public const SWITCH_PROXY = 306;
    
    /**
     * @var integer
     */
    public const TEMPORARY_REDIRECT = 307;
    
    /**
     * @var integer
     */
    public const PERMANENT_REDIRECT = 308;
    
    /**
     * @var integer
     */
    public const BAD_REQUEST = 400;
    
    /**
     * @var integer
     */
    public const UNAUTHORIZED = 401;
    
    /**
     * @var integer
     */
    public const PAYMENT_REQUIRED = 402;
    
    /**
     * @var integer
     */
    public const FORBIDDEN = 403;
    
    /**
     * @var integer
     */
    public const NOT_FOUND = 404;
    
    /**
     * @var integer
     */
    public const METHOD_NOT_ALLOWED = 405;
    
    /**
     * @var integer
     */
    public const NOT_ACCEPTABLE = 406;
    
    /**
     * @var integer
     */
    public const PROXY_AUTHENTICATION_REQUIRED = 407;
    
    /**
     * @var integer
     */
    public const REQUEST_TIME_OUT = 408;
    
    /**
     * @var integer
     */
    public const CONFLICT = 409;
    
    /**
     * @var integer
     */
    public const GONE = 410;
    
    /**
     * @var integer
     */
    public const LENGTH_REQUIRED = 411;
    
    /**
     * @var integer
     */
    public const PRECONDITION_FAILED = 412;
    
    /**
     * @var integer
     */
    public const REQUEST_ENTITY_TOO_LARGE = 413;
    
    /**
     * @var integer
     */
    public const REQUEST_URI_TOO_LARGE = 414;
    
    /**
     * @var integer
     */
    public const UNSUPPORTED_MEDIA_TYPE = 415;
    
    /**
     * @var integer
     */
    public const REQUESTED_RANGE_NOT_SATISFIABLE = 416;
    
    /**
     * @var integer
     */
    public const EXPECTATION_FAILED = 417;
    
    /**
     * @var integer
     */
    public const MISDIRECTED_REQUEST = 421;
    
    /**
     * @var integer
     */
    public const UNPROCESSABLE_ENTITY = 422;
    
    /**
     * @var integer
     */
    public const LOCKED = 423;
    
    /**
     * @var integer
     */
    public const FAILED_DEPENDENCY = 424;
    
    /**
     * @var integer
     */
    public const UNORDERED_COLLECTION = 425;
    
    /**
     * @var integer
     */
    public const UPGRADE_REQUIRED = 426;
    
    /**
     * @var integer
     */
    public const PRECONDITION_REQUIRED = 428;
    
    /**
     * @var integer
     */
    public const TOO_MANY_REQUESTS = 429;
    
    /**
     * @var integer
     */
    public const REQUEST_HEADER_FIELDS_TOO_LARGE = 431;
    
    /**
     * @var integer
     */
    public const UNAVAILABLE_FOR_LEGAL_REASONS = 451;
    
    /**
     * @var integer
     */
    public const INTERNAL_SERVER_ERROR = 500;
    
    /**
     * @var integer
     */
    public const NOT_IMPLEMENTED = 501;
    
    /**
     * @var integer
     */
    public const BAD_GATEWAY = 502;
    
    /**
     * @var integer
     */
    public const SERVICE_UNAVAILABLE = 503;
    
    /**
     * @var integer
     */
    public const GATEWAY_TIME_OUT = 504;
    
    /**
     * @var integer
     */
    public const HTTP_VERSION_NOT_SUPPORTED = 505;
    
    /**
     * @var integer
     */
    public const VARIANT_ALSO_NEGOTIATES = 506;
    
    /**
     * @var integer
     */
    public const INSUFFICIENT_STORAGE = 507;
    
    /**
     * @var integer
     */
    public const LOOP_DETECTED = 508;
    
    /**
     * @var integer
     */
    public const NOT_EXTENDED = 510;
    
    /**
     * @var integer
     */
    public const NETWORK_AUTHENTICATION_REQUIRED = 511;
    
    
    /**
         * getReasonPhrase
         * @param int $value
         * @return string
         */
    public static function getReasonPhrase( int $value) : string { }
    
}


```

## Examples

