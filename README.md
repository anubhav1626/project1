# project1

First job:
In this job, I clone my GitHub repo (Dev branch) to my 1st docker container. This is used for testing purposes. If this job executes successfully then the code pushed by the developer is good.
Whenever some changes in code uploaded to my GitHub(Dev1 branch), this job automatically triggered.


Second Job:
In this job, I clone my GitHub repo (Master branch) to 2nd docker container. This is our main branch so we use this container to deploy our website.
Whenever some changes happens in code (Master branch) to my GitHub, this job automatically triggered .


Third Job:
This job is triggered by job1 if job1 is successfully executed.
We merge Dev1 to Master branch and trigger Job2 so that our production system clone the latest commit and deploy a website.
