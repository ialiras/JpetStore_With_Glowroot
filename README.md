# JpetStore_With_Glowroot

JPetStore Instrumentations with Glowroot Profiler in Docker image: 

Hi Connection, 

I have created Docker image for Jpetstore web application along with glowroot java profiler. 

 ![glowroot](https://user-images.githubusercontent.com/10634825/194889809-d6afb8b2-1117-4ea8-b5a0-fb86b52901a4.png)


Installation Steps: 

Install docker on window/linux system 

Pull image and run image as below: 

docker run -p 8080:8080 -p 4000:4000 -d ialiras/jpetstore_glowroot 

To monitor application host metric run the command: 

Docker exec  - it  <container name> /bin/bash 

  

With the help of this image anyone can learn performance engineering concepts like below, 

High response time RCA 

Monitor JAVA Mbeans like below 

Thread pool  

JDBC connection  

GC time  

Heap memory  utilization 

Thread dump analysis  

Method level instrumentation. 

Monitor host by linux commands: 

top command  

 vmstat  

Iostat 

netstat  

pidstat. 

 

 

 
