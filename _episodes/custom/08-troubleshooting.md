## On our system

> interactive jobs

The HTCondor log file, as well as the output and error files, can contain
valuable information about your jobs 

<p>The log file contains information that HTCondor tracks for each job, including 
when it was submitted, started, and stopped.  It also describes resource use, 
and where the job ran. </p>

  <ul>
    <li>When jobs were submitted, started, and stopped: 
    <pre>000 (16173120.000.000) 03/16 09:50:48 Job submitted from host: 
    <128.104.101.92:9618?addrs=128.104.101.92-9618</pre>
    <pre>001 (16173120.000.000) 03/16 09:53:10 Job executing on host: 
    <128.105.244.92:9618?addrs=128.105.244.92-9618&noUDP&sock=7150_4f71_3></pre>
    <pre>005 (16173120.000.000) 03/16 09:58:12 Job terminated.</pre></li>
    <li>Resources used
    <pre>Partitionable Resources :    Usage  Request Allocated
Cpus                 :                 1         1
Disk (KB)            :       15  1048576  11053994
Memory (MB)          :        1   102400    102400</pre></li>
    <li>Exit status
    <pre>(1) Normal termination (return value 0)</pre>
    A return value of "0" is normal; non-zero values indicate an error.</li>
    <li>Where the job ran: 
    <pre>Job executing on host: <128.105.244.92:</pre>
    You can get the "name" of the machine where a job ran by running the command 
    <code>host</code>, followed by the 4-part IP address.  Using the above 
    example, this would look like: 
    <pre>$ host 128.105.244.92</pre> </li>
  </ul>

> ## Exercise
> 
> run interactive job
>
{: .challenge} 
