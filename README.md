# Basics of Vertical and horizontal scaling In systems
## Introduction
When designing enterprise-grade applications scalability is the biggest concern of all. As your application grows you need to handle more and more requests for the service you are providing through your application. To serve those requests you need more than a typical computer that you use in your day to day life. You need a powerful machine to act as an endpoint to your application. We call that machine a server. A server is just a machine with typically more computation power which is geared towards the use of resources carefully and efficiently. Those resources might be Space, CPU time, etc.

## What is Scaling?
As we talked about in the previous paragraph that, scalability is the biggest concern of growing applications. Then what do we mean by Scaling? Scaling in system design means upgrading your current hardware and computation capability of your server. Scaling is just this it allows you to handle more and more request to your service by adding more and more computation power to your server that computation power can be achieved by following two ways.
### 1. Vertical Scaling 
Scaling vertically means, upgrading your existing server with more processing power, memory, and other necessary resources. Vertical Scaling is just building a very powerful machine that can handle the traffic you are facing. But there is a limit to how much you can vertically scale. Because there is a hardware limit to the machine.
### 2. Horizontal Scaling
Scaling horizontally means, buying more machines and using them over a network. Requests from users can be forwarded to those machines over a network by selecting an idle server for that request. We can loosely attach more machines to handle more traffic at any time. 

Both of the above Scalings have their advantages and disadvantages some of which I'll list below.

#### **Horizontal Scaling Advantages and Disadvantages**:
* It provides a faster response because IPC is used.
* Easier to set up and handle.
* Data is consistent
* Costly in terms of money.
* single point of failure. Shutting down of server can result in the drop of service.
* Has a hardware limit.
#### **Vertical Scaling Advantages and Disadvantages**:
* Loosely coupled, hence easy to remove and add more servers.
* Resilient towards failure
* RPC is used hence a slower response to the user.
* Load Balancing is required. 
* Data inconsistency
* Scales easily compared to horizontal

### Conclusion:
In a real-world scenario, both of the above scaling methods are used. We pick the positives of both the vertical and horizontal scaling and use them to build robust systems. Hence if you want your system to scale and also be fast use both. But Horizontal scaling requires a lot more effort and skills to build, hence there are services like AWS, AZURE, etc. to aid that need for their users.


#### references
* https://medium.com/@spencerwgoodman/vertical-and-horizontal-scaling-in-system-design-718cabb80a1a
* https://www.youtube.com/watch?v=xpDnVSmNFX0
* https://www.youtube.com/watch?v=K0Ta65OqQkY
