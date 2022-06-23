# cq-quickstart-6.5.0-standalone-quickstart.jar

## Where

- crx-quickstart/app/cq-quickstart-6.5.0-standalone-quickstart.jar

## What

- Standalone Java Application launcher for Sling

## Remarks

- This JAR file is different from the AEM installation JAR file.

```
$ java -jar cq-quickstart-6.5.0-standalone-quickstart.jar -h
usage: org.apache.sling.launchpad.app.Main [ start | stop | status ] [ -j adr ] [ -l loglevel ] [ -f logfile ] [ -c slinghome ] [ -i launchpadhome ] [ -a address ] [ -p port ] { -Dn=v } [ -h ]
    start         listen for control connection (uses -j)
    stop          terminate running Apache Sling (uses -j)
    status        check whether Apache Sling is running (uses -j)
    threads       request a thread dump from Apache Sling (uses -j)
    -j adr        host and port to use for control connection in the format '[host:]port' (default 127.0.0.1:0)
    -l loglevel   the initial loglevel (0..4, FATAL, ERROR, WARN, INFO, DEBUG)
    -f logfile    the log file, "-" for stdout (default logs/error.log)
    -c slinghome  the sling context directory (default sling)
    -i launchpadhome  the launchpad directory (default slinghome)
    -a address    the interfact to bind to (use 0.0.0.0 for any)
    -p port       the port to listen to (default 8080)
    -r path       the root servlet context path for the http service (default is /)
    -n            don't install the shutdown hook
    -Dn=v         sets property n to value v. Make sure to use this option *after* the jar filename. The JVM also has a -D option which has a different meaning
    -h            prints this usage message
```

## See Also

- [bin/start](/crx-quickstart/bin/start.md)

