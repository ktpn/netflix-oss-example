#Netflix OSS Example

##Introduction

This repo contains an example of Sping cloud (Netflix OSS) micro-services architecture.

The main objective is to test how the micro-services use the discovery service (Eureka), the configuration service and the load balancing (Ribbon).
 
The example contains the following components:

1. [Eureka] (https://github.com/Oreste-Luci/netflix-oss-example/tree/master/eureka-server)
2. [Config Service] (https://github.com/Oreste-Luci/netflix-oss-example/tree/master/config-service)
3. [Turbine] (https://github.com/Oreste-Luci/netflix-oss-example/tree/master/turbine)
4. [Hystrix] (https://github.com/Oreste-Luci/netflix-oss-example/tree/master/hystrix-dashboard)
5. [Microservice C: This is the server micro-service for service B] (https://github.com/Oreste-Luci/netflix-oss-example/tree/master/service_c)
6. [Microservice B: This is the server micro-service for service A] (https://github.com/Oreste-Luci/netflix-oss-example/tree/master/service_b)
7. [Microservice A: This is the client micro-service] (https://github.com/Oreste-Luci/netflix-oss-example/tree/master/service_a)

The services can be started in any other but it recommended to start them in above order.

Service A exposes endpoints that in turn call service B endpoints and service B will call service C endpoints. The clien services find the server services via Eureka.

There is further documentation for each component in the links above.

##Further Reading

* [Spring Cloud] (http://projects.spring.io/spring-cloud/spring-cloud.html)
* [Dynamic configuration management with Spring Cloud Config] (http://qiita.com/making@github/items/704d8e254e03c5cce546)
* [Spring Cloud Netflix] (http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html)
* [Microservice Registration and Discovery with Spring Cloud and Netflix's Eureka] (https://spring.io/blog/2015/01/20/microservice-registration-and-discovery-with-spring-cloud-and-netflix-s-eureka)
* [Netflix Ribbon] (https://github.com/Netflix/ribbon/wiki)


> **Note:**
> This example is using Spring Boot version 1.2.3.RELEASE and Spring Cloud version 1.0.0.RELEASE.
