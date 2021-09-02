# ReadMe
## Comparison of runtimes
**Real**
refers to actual elapsed time, i.e. time from start to finish. This is all elapsed time including time slices used by other processes and time the process spends blocked (for example if it is waiting for I/O to complete).\
**User** and **Sys** refer to CPU time used only by the process.Real is wall clock time - time from start to finish of the call. \
**User** is the amount of CPU time spent in user-mode code (outside the kernel) within the process. This is only actual CPU time used in executing the process. Other processes and time the process spends blocked do not count towards this figure.\
**Sys** is the amount of CPU time spent in the kernel within the process. This means executing CPU time spent in system calls within the kernel, as opposed to library code, which is still running in user-space.\
As we can see, in real time which is the actual execute time, the parallel time is the half of serial time, because I have two CPUs in my VM which makes sense.
Also, when running the executable file, I also monitor the CPU running percentage. Parallel time %CPU is twice as serial time.


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
Open-source
