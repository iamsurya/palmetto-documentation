---
title: How to run jobs that take more than 72/168 hours
keywords: [long,walltime]
sidebar: documentation_sidebar
permalink: userguide_howto_run_long_jobs.html
---

Currently,
jobs are limited to walltime of 72 hours (phases 7 and up exclude phase 8c)
and 168 hours (phases 1-6 and 8c).
If you expect that your computations may take
more time, you have several options:

* **Checkpoint** your application: this approach is often
useful in large/long-running simulations. Often it is possible
to periodically save intermediate results from the application,
so that after a job terminates, the application can be "restarted"
from the latest saved results.

* **Optimize** your application: it is often possible to obtain
better performance by various means, such as parallelizing
serial programs, using GPUs, optimizing I/O, etc.,
The first step in such optimization is always
to identify bottlenecks, i.e., identifying which portion(s)
of the application/program is/are the largest contributor
to the running time. You are welcome to visit the Office Hours
or schedule a meeting with our research support staff
to discuss optimization

* [Submit a **reservation request**]({{site.baseurl}}/userguide_howto_submit_reservation_request.html)
