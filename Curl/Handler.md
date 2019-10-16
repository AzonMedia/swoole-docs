# Swoole\Curl\Handler

## Intrduction

## API

```php
<?php

namespace Swoole\Curl;

/**
 * Class Handler
 * @package Swoole\Curl
 */
class Handler
{

    private const ERRORS = [
        CURLE_URL_MALFORMAT => 'No URL set!',
    ];


    /**
     * @var Client
     */
    private $client;
    
    /**
     * @var array
     */
    private $info = array (
      'url' => '',
      'content_type' => '',
      'http_code' => 0,
      'header_size' => 0,
      'request_size' => 0,
      'filetime' => -1,
      'ssl_verify_result' => 0,
      'redirect_count' => 0,
      'total_time' => 5.3E-5,
      'namelookup_time' => 0.0,
      'connect_time' => 0.0,
      'pretransfer_time' => 0.0,
      'size_upload' => 0.0,
      'size_download' => 0.0,
      'speed_download' => 0.0,
      'speed_upload' => 0.0,
      'download_content_length' => -1.0,
      'upload_content_length' => -1.0,
      'starttransfer_time' => 0.0,
      'redirect_time' => 0.0,
      'redirect_url' => '',
      'primary_ip' => '',
      'certinfo' => 
      array (
      ),
      'primary_port' => 0,
      'local_ip' => '',
      'local_port' => 0,
      'http_version' => 0,
      'protocol' => 0,
      'ssl_verifyresult' => 0,
      'scheme' => '',
    );
    
    /**
     * @var bool 
     */
    private $withHeaderOut = false;

    /**
     * @var bool
     */
    private $withFileTime = false;

    /**
     * @var 
     */
    private $urlInfo;
    
    /**
     * @var 
     */
    private $postData;
    
    /**
     * @var 
     */
    private $outputStream;
    
    /**
     * @var 
     */
    private $proxy;
    
    /**
     * @var array
     */
    private $clientOptions = [];
    
    /**
     * @var bool
     */
    private $followLocation = false;
    
    /**
     * @var 
     */
    private $maxRedirs;
    
    /**
     * @var bool
     */
    private $withHeader = false;

    /**
     * @var bool
     */
    private $nobody = false;
    
    /** 
     * @var callable 
     */
    private $headerFunction;
    
    /** 
     * @var callable 
     */
    private $readFunction;
    
    /** 
     * @var callable 
     */
    private $writeFunction;
    
    /** 
     * @var callable 
     */
    private $progressFunction;
    
    /**
     * @var bool
     */
    public $returnTransfer = false;
    
    /**
     * @var string
     */
    public $method = 'GET';
    
    /**
     * @var array
     */
    public $headers = [];
    
    /**
     * @var int
     */
    public $errCode = 0;
    
    /**
     * @var string
     */
    public $errMsg = '';
    
    
    /**
     * @var array
     */
    private const ERRORS = array (
      3 => 'No URL set!',
    );
    
    
    /**
     * @param type $url
     * @return void
     */
    public function __construct( $url = NULL) { }
    
    /**
     * @param string $url
     * @return void
     */
    private function create( string $url) : void { }
    
    /**
     * 
     * @return void
     */
    public function execute( ) { }
    
    /**
     * 
     * @return void
     */
    public function close( ) : void { }
    
    /**
     * @param type $code
     * @param type $msg
     * @return void
     */
    private function setError( $code, $msg = '') : void { }
    
    /**
     * 
     * @return string
     */
    private function getUrl( ) : string { }
    
    /**
         * @param int $opt
         * @param $value
         * @return bool
         * @throws Swoole\Curl\Exception
         */
    public function setOption( int $opt, $value) : bool { }
    
    /**
     * 
     * @return void
     */
    public function reset( ) : void { }
    
    /**
     * 
     * @return void
     */
    public function getInfo( ) { }
    
    /**
     * @param array $parsedUrl
     * @return string
     */
    private function unparseUrl( array $parsedUrl) : string { }
    
    /**
     * @param string $location
     * @return array
     */
    private function getRedirectUrl( string $location) : array { }
    
}


```

## Examples

