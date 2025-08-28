# nincat
A basic netcat in bash

```
Usage: ./nincat [options] <host> <port>

Options:
  -c           Send CRLF as line-ending.
  -u           Use UDP instead of TCP.
  -z           Zero-I/O mode, just scan for open ports.
  -w <sec>     Timeout for connections.
  --no-color   Disable ANSI colors.
  -h, --help   Show this help.

Examples:
  ./nincat example.com 80
  ./nincat -c example.com 80 <<< 'GET / HTTP/1.0'
  ./nincat -u 192.168.1.1 53
  ./nincat -z -w 5 example.com 22
  ./nincat whois.ripe.net 43
```
