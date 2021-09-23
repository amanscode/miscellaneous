# Miscellaneous stuff

## JMap


Add below option to JAVA_OPTS:
```bash
-XX:+PrintClassHistogram
```

To see heap histogram use below command:
```bash
jmap -histo <process_id>
```
The output shows the total size and instance count for each class type in the heap.

To create a heap dump, use below command:
```bash
jcmd <process_id> GC.heap_dump <filename>
```

Link:
https://docs.oracle.com/en/java/javase/15/troubleshoot/troubleshoot-memory-leaks.html#GUID-06976380-65AC-4455-BBFC-94BC02A42BBC
