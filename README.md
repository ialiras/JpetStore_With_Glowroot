# JpetStore Glowroot Docker image

Hi All, 

I have created a Docker image for the Jpetstore web application along with a Glowroot Java Profiler. For those who are interested in learning about application performance engineering concepts like identifying high response time RCA, JDBC connection pool issues, memory leaks, and high CPU utilisation ,high GC pause time , out of memory issues,thread contention,thread blocking & high DB query execution time.

Run the load test using the provided Jmeter JMX script(jpetstore.jmx), increase the number of users, and see the Jpetstore application behaviour using glowroot java profiler http://localhost:4000 



 ![glowroot](https://user-images.githubusercontent.com/10634825/194889809-d6afb8b2-1117-4ea8-b5a0-fb86b52901a4.png)


## Installation Steps: 

Install docker on window/linux system 

Pull image and run image as below: 

`docker run -p 8080:8080 -p 4000:4000 -d ialiras/jpetstore_glowroot`

To monitor application host metric run the command: 

`docker exec  - it  <container ID> /bin/bash`

Launch Application http://localhost:8080/mybatis-jpetstore-6.0.1/actions/Catalog.action ![jpet](https://user-images.githubusercontent.com/10634825/194901885-aeccb103-2508-44b5-ae0d-4945889b30bc.png)

Launch Glowroot http://localhost:4000 ![glowrrott](https://user-images.githubusercontent.com/10634825/194902433-27a5812c-2c15-4db8-8d09-8644fcfc6645.png)




With the help of this image anyone can learn performance engineering concepts like below, 

- High response time RCA 

- Monitor JAVA Mbeans like below 

  - Thread pool  

  - JDBC connection  

  - GC time  

  - Heap memory  utilization 

  - Thread dump analysis  

  - Method level instrumentation. 

- Monitor host by linux commands: 

  - top command  

  - vmstat  

  - iostat 

  - netstat  

  - pidstat. 

 

 

 
