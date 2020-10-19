# Application Load Balancer

* The **Application Load Balancer** has some enhanced features over the **Classic Load Balancer**

  * Supported Protocols
  * CloudWatch Metrics
  * Access Logs
  * Health Checks
  * Enable additional routing mechanisms using path and host-based routing
    * Path-based provides rules that forward requests to different target groups
    * Host-based can be used to define rules that forward requests to different target groups based on host name
  * Native IPv6 Support
  * AWS Web Application Firewall (WAF) integration
  * Dynamic Ports
    * Amazon ECS integrates with Application Load Balancer to expose Dynamic Ports utilized by scheduled containers
  * Deletion protection and request tracing
    * Request tracing can be used to track HTTP requests from clients to target
  * HTTP2 and WebSocket support
* When to use the Application Load Balancer?

  * Use containers to host microservices and route to those applications from a single load balancer
  * Allows you to route different requests to the same instance, but differ the path based on the port
  * If you have various different containers listening on various ports, you can set up routing rules to distribute traffic to only the desired backend application
* New Terms


  | Concept | Description |
  | - | - |
  | Listeners | A listener is a process that checks for connection requests, using the protocol and the port that you configure. The rules that you define for a listener determine how the load balancer routes requests to the targets in one or more groups. |
  | Target | A target is a destination for traffic based on the established listener rules. |
  | Target Group | Each target group routes requests to one or more registered targets using the protocol and port number specified. A target can be registered with multiple target groups. Health checks can be configured on a per target group basis. |
* The Application Load Balancer registers targets instead of instances
* A target group is how the targets are registed to the load balancer
* Define rules for the listeners in order to direct how the requests received by the load balancer are routed to the backend targets
* Targets can be members of multiple target groups
