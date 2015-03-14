Tool for copying ZooKeeper data from one cluster to another. You can use many threads - this will speed up copying process.
Tool will be useful in cases when there are big network latency and huge data set. Single-threaded method in this case requires too much time.

Current version usage:
```

java 
    -Dlogger.config="log4j.properties" 
    -Dsource="server:port/path" 
    -Ddestination="server:port/path" 
    -Dthreads=10 
-jar zkcopy.jar

```