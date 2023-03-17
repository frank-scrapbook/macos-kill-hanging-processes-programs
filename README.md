# macos-kill-hanging-processes-programs
macOS tips on killing hanging processes/programs (applications)

### Search for process id (pid)
```
ps -ax | grep <application_name>
```

E.g. 
```
ps -ax | grep virtualbox
```

### ALTERNATIVE: use activity monitor to locate the active window of the application for the pid

### Terminal
```
kill <pid>
```

OR

```
kill -9 <pid>
```

E.g.
```
kill -9 3201
```

NOTE: the -9 is to indicate the signal is SIGKILL (return code 9)
