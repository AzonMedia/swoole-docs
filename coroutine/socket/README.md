# Coroutine Socket

## API

```php
funcion __construct( domain,  type,  protocol)
funcion bind( address,  port)
funcion listen( backlog)
funcion accept( timeout)
funcion connect( host,  port,  timeout)
funcion recv( length,  timeout)
funcion recvPacket( timeout)
funcion send( data,  timeout)
funcion sendFile( filename,  offset,  length)
funcion recvAll( length,  timeout)
funcion sendAll( data,  timeout)
funcion recvfrom( peername,  timeout)
funcion sendto( addr,  port,  data)
funcion getOption( level,  opt_name)
funcion setProtocol(array settings)
funcion setOption( level,  opt_name,  opt_value)
funcion shutdown( how)
funcion cancel( event)
funcion close()
funcion getpeername()
funcion getsockname()
```