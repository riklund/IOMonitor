[![Build Status](https://travis-ci.org/riklund/IOMonitor.png)](https://travis-ci.org/riklund/IOMonitor)

#IOMonitor: a cheapskate iotop alternative
The iotop tool usually requires root privileges to run or some fiddling with config files by root. These scripts provide a way to monitor the I/O o a single process.

##Installation
Copy the script files to a directory in your $PATH.

##Usage

To monitor a process, issue 

```bash
iodisp PID
```
where PID is the process ID of a running process to monitor, OR

```bash
iolock process-name
```

to monitor a process with the name _process-name_. If at any time there are more than one process matching process-name, there will be no output, and likewise if there are no process matching that name. The program will then silently wait for the number of matching processes to become one.