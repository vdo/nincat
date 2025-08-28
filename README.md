# nincat 🐈‍⬛
A basic TCP netcat in bash

## Usage

```
Usage: ./nincat [options] <host> <port>

Options:
  -c           Send CRLF as line-ending.
  -z           Zero-I/O mode, just scan for open ports (TCP only).
  -w <sec>     Timeout for connections.
  --no-color   Disable ANSI colors.
  -h, --help   Show this help.

Examples:
  ./nincat example.com 80
  ./nincat -c example.com 80 <<< 'GET / HTTP/1.0'
  ./nincat -z -w 5 example.com 22
  ./nincat -c whois.ripe.net 43 <<< "example.com"

```

## License
Licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE) for details.

## Platform Support
⚠️ **Linux only** - This tool is designed for Linux systems and is not supported on macOS.