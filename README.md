# Infra-modernization
Infra modernization Public Cloud GCP/AWS

#company Name: Enterprise Pharma company us based 
#problem statement:Food Pharma company Moving thier workload from onprimes to Public cloud due to data center exist and to increase the performance of worklaods.
1)we followed Lift and shift approch for E-commerce webiste to move to cloud.
2) Attended couple of workshops with client to understand the pain area and did internal assesment with the help of client infrasture team to discover the inventory by using starta zone tool to scan the internal servers application scan and db scan.
once we got the overall inventory.

3)we started providing solution considering the lift and shift approch 
4)with creating compute engine & custom machine type with optimal cpu and memory utilization
5) Suggested to host thier workload Ecommerce web application in compute engine with MIG for autoscaling application load balancer. within zone and regions

6) And from Database perpective  to be hosted in cloud sql instead of hosting on compute engine so that you dont have to worry about the adminstration and performance
of db based on demand it can be scale-in and scale out. 
7) So this E commerce application reading more than the writing.  its retail E-commerce appllication where customer going search the products and it to the catalog which means read than write IOPS is required hence i introduce the read replica with the synchronour replication across the instances.
8) i can also introduce caching from the content perspective which can cover the HA perpective and laod the of the site
9) Now all frontend and middleware is place in autoscalling thats where it will scale based on the request coming in scale in scale out automcatically
10) I'm able to cover the availibility scalability  of fronted and middleware and backedn i'm using pass services which scale automatically 
11) Cachin i'm able to respond to the user quickly when there is seach of the same object happend this how my approch would be on HA.
12) Now i also introuduce the security aspect for the user interacting user with my application securely integrate with openIDP for authencticate the services
13) attack can happen from anywhere so i will also introduce WAF/Cloud armor to ensure that sql scripting attack or any ddos attack can be filtered any malicious attack

14) also my application sits within the vpc and i enable 
                      1) vpc flow logs
                      2) audit logs
                      3) DNs logs
                      4) cloud trail logs
                      5) network logs
                     so that i can prevent it or track who's has done what
                     
                 15) by considering all this aspect i'm able to build the scalable environment where user going to increase, since i have build autoscalling for VM
                 and Pass service automatically it can respond to the user
                 
  15) now you are also mentiong that the user is try to access this globally, now i'm able to build this solution in USA i'll try to replicate same architecture in Europe as well with multi region because to restrict the data soverinty of customer access from the other part of the world and GDPR perspective.
  and customer privact to ensure that data leakage is protected so because of that decided to go with multi region solution.
  
                
