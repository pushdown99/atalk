## Problem

~~~console
Time limited <->
Jitsi meet capacity: 100 participants
~~~

## Documents
https://meetrix.io/blog/webrtc/jitsi/how-many-users-does-jitsi-support.html

### How many users can one Jitsi conference support?
~~~console
As Jitsi relays video streams from one user to all other users in multiple bit rates according to available bandwidths and network speeds, most performance related issues would occur on the user machines rather than the Jitsi video bridge it self.

We recommend upto 100 users per conference with about 30% on video. If the users machines are Core i5/i7 and the network infrastructure has good specifications Jitsi meetings can accommodate ~50 video users with 75-100 users all total (balance users with audio only). We can also configure Jitsi webconference mode where 250-500 users can easily participate and listen and see one presenter is also possible.
~~~

### How many concurrent meetings and concurrent users can Jitsi handle?
~~~console
Jitsi video bridges and Jibri video stream recorders can be auto-scaled on demand user Kubernetes or AWS cloudwatch services and geographically optimized using Octo upon a HA-proxy load balanced multi-shard setup. This can theoretically support unlimited user conferences. But most business would not require very large clusters and even one shard could be well enough for small or medium enterprises.
~~~

### What servers should Jitsi be setup on?
~~~console
On AWS we recommend 8 core or 16 core server instances with 8 or 16GB of RAM for JVBs. T3 Large, C5XLarge, C52XLarge of even high compute powered servers need to configured case by case considering performance and cost.
~~~

### What performance matrices should be considered?
~~~console
CPU and RAM on servers as well the in/out bandwidth quality and limitations would impact your Jitsi service quality. Load testing your rigs for highly available on-demand services is also recommended.
~~~