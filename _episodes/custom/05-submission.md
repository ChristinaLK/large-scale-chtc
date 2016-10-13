## On our system

Submit file example: (`hello-chtc.sub`)

~~~
universe = vanilla
log = hello-chtc_$(Cluster).log
error = hello-chtc_$(Cluster)_$(Process).err

executable = hello-chtc.sh
arguments = $(Cluster) $(Process)
output = hello-chtc_$(Cluster)_$(Process).out

should_transfer_files = YES
when_to_transfer_output = ON_EXIT
# transfer_input_files = file1,/absolute/pathto/file2,etc

request_cpus = 1
request_memory = 1GB
request_disk = 1MB
queue 3
~~~

Simple shell script executable: (`hello-chtc.sh`)

~~~
#!/bin/bash

sleep = 120
echo "Hello from Job $1.$2 running as `user`@`hostname
~~~

To submit a job, run the command: 

~~~
$ condor_submit hello-chtc.sub
~~~

> ## Exercise
> 
> Making a copy of the submit file and script above, submit them 
> as a job.  
>
{: .challenge} 
