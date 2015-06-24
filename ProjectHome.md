**SIEGE-3.0.5 for windows** compiled using Cygwin, tested under windows 7 home premium 64bit and windows XP 32bit

**ABOUT SIEGE**

Siege is an http load testing and benchmarking utility. It was designed to let web developers measure their code under duress, to see how it will stand up to load on the internet. Siege supports basic authentication, cookies, HTTP and HTTPS protocols. It lets its user hit a web server with a configurable number of simulated web browsers. Those browsers place the server “under siege.”


**INSTALLATION**

  1. Download [siege-windows-3.0.5.zip](https://siege-windows.googlecode.com/svn/trunk/siege-windows-3.0.5.zip)
  1. Extract to C:\siege-windows and you're done.
  1. if you want to place siege other then directory above, rename and move siege configuration file **siege-windows\etc\siegerc** to **C:\Users\YOUR-USERNAME\.siegerc** (Windows 7) it is very important the file **.siegerc** must be started with the dot "."

**Benchmark Test Example**

- test benchmark http://127.0.0.1 with concurrent thread (connection) 10 for 60 seconds

```
siege -c10 -t60s http://127.0.0.1
```

- test benchmark http://127.0.0.1 with no limit concurrent thread (connection) for 60 seconds

```
siege -b -t60s http://127.0.0.1
```

**USAGE & OPTION**

Usage: siege [options](options.md)
> siege [options](options.md) URL
> siege -g URL
Options:
> -V, --version             VERSION, prints the version number.

> -h, --help                HELP, prints this section.

> -C, --config              CONFIGURATION, show the current config.

> -v, --verbose             VERBOSE, prints notification to screen.

> -q, --quiet               QUIET turns verbose off and suppresses output.

> -g, --get                 GET, pull down HTTP headers and display the transaction. Great for application debugging.

> -c, --concurrent=NUM      CONCURRENT users, default is 10

> -i, --internet            INTERNET user simulation, hits URLs randomly.

> -b, --benchmark           BENCHMARK: no delays between requests.

> -t, --time=NUMm           TIMED testing where "m" is modifier S, M, or H. ex: --time=1H, one hour test.

> -r, --reps=NUM            REPS, number of times to run the test.

> -f, --file=FILE           FILE, select a specific URLS FILE.

> -R, --rc=FILE             RC, specify an siegerc file

> -l, --log[=FILE]          LOG to FILE. If FILE is not specified, the default is used: PREFIX/var/siege.log

> -m, --mark="text"         MARK, mark the log file with a string.

> -d, --delay=NUM           Time DELAY, random delay before each requst between 1 and NUM. (NOT COUNTED IN STATS)

> -H, --header="text"       Add a header to request (can be many)

> -A, --user-agent="text"   Sets User-Agent in request

> -T, --content-type="text" Sets Content-Type in request



More Information visit author of siege http://www.joedog.org/siege-home/

created by: www.prpagerank.com [Check Pagerank](http://www.prpagerank.com)