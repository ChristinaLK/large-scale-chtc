---
title: "Jobs and Scheduling"
teaching: 15
exercises: 0
questions:
- "What have I logged into?"
objectives:
- "Draw a diagram of the compute system that you're using."
- "Describe the role of a batch scheduler."
keypoints:
- "A job consists of a computational task, usually defined by input data and a piece of software, producing output data."  
- "Most large scale systems consist of a head node for logging in and submitting jobs, where jobs are performed on worker nodes."  
- "A batch scheduler controls where and when jobs run on the worker nodes."  
---

> define a job

> define structure of large scale system (head node + worker nodes)

> describe the role of a scheduler

> describe the very basics of how schedulers work 
> (submit file, queue of tasks, allocation of resources)

{% include_relative custom/04-scheduler-basics.md %}
