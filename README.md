# bulkbuster
A DOS tool that can be used to stress test the HTTP server
Bulkbuster DoS tool
=============

BulkBuster DoS tool written in both Go and Python


This tool targeted for stress testing and may really down badly configured server or badly made app. Use it carefully.

Examples:

    $ bulkbuster -site http://example.com/test/ 2>/dev/null

    $ BBMAXPROCS=4096 bulkbuster -site http://example.com 2>/tmp/errlog

Useful environment vars:

* GOMAXPROCS
  Set it to number of your CPUs or higher (no more actual for latest golang versions).
* BBMAXPROCS
  Limit the connection pool (1024 by default).

