# Microservices

Expectations from a Microservice.   
1. programing language indepedently 
2. deploy independently.   
3. scale independently.    
4. team work independently.   
5. fault tolerance.    

## Best practices for building a Microsercices.

### Use single reponsibility principle.   
let see example how to devide responsibilites with example.

food delivery service
1. Inventory service.
2. order service.
3. Payment service.   
4. User profile service.   
5. Delivery notification service.

### Create separate data store(s) for your Microservice.  

<img src="assets/separate_data_store.png"  width="392.5" height="285.5">


### Use Asynchronius communication to achieve  loose coupling.   

<img src="assets/loose_coupling.png"  width="392.5" height="172.78">


### Use a circuit breaker to achieve fault tolerance.   

<img src="assets/circuite_breaker.png"  width="392.5" height="79.87">


when someother-service wait more time then order-service return default result to inventory-service for make fault tolerance.   

### Proxy your Microservice requests throught an API Gateway.   

<img src="assets/proxy.png"  width="392.5" height="251.06">

can reject unauthorized requests from the api gateway before reach your microservice.    

### Version your microservice for breaking changes.    

<img src="assets/multiple_versions.png"  width="392.5" height="163.101">   

new version of your end point while continuing to support older versions.   