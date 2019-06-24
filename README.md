# hystrix-turbine-dashboard
centralized hystrix dashboard - using turbine stream

 - Hystrix dashboard  
   ![./hystrix-dashboard.png](./hystrix-dashboard.png)
 
 - Hystrix dashboard - centralized - using turbine  
   ![./hystrix-dashboard-turbine.png](./hystrix-dashboard-turbine.png)
 
 - Hystrix dashboard - centralized - using turbine + stream(rabbitmq)  
   ![./hystrix-dashboard-turbine-stream.png](./hystrix-dashboard-turbine-stream.png)

# Bug:

```
<springboot.version>2.1.6.RELEASE</springboot.version>
<springcloud.version>Greenwich.SR1</springcloud.version>

or

<springboot.version>2.1.5.RELEASE</springboot.version>
<springcloud.version>Greenwich.RELEASE</springcloud.version>
```

Have to remove spring-boot-starter-actuator from pom.xml, otherwise, cannot register turbine.stream.destination: hystrixStreamOutput and no data displayed on hystrix dashboard

_refer to http://blog.didispace.com/spring-cloud-starter-dalston-5-2_