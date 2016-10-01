## On our system

~~~
universe = vanilla
queue 3
~~~

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
