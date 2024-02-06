# Coding for Coding: Web Development Showcase

Welcome to the Coding for Coding repository, a showcase for various web development techniques and practices without the constraints of real-world application requirements.

# What Techniques have been used?

## HTTP Response Status Codes

This demonstrates the implementation of practical HTTP response status codes. Some codes have been intentionally omitted due to the following responses: 1) They are deprecated, like 102 Processing; or 2) They are inapplicable for a backend server, like 103 Early Hints.

- [ ] 100 Continue: When uploading large files where the client needs to ensure server readiness to accept large data payloads, `100 Continue` status code is used. The client sends Expect: 100-Continue header and waits for the server to respond with 100 Continue before starting to send actual data.
  - [AWS S3 POST example](https://docs.aws.amazon.com/AmazonS3/latest/API/RESTObjectPOST.html)
- [ ] 101 Switching Protocols: When initiating a WebSocket connection, this status code comes into play. Clients propose an upgrade in protocol from HTTP to WebSocket by sending a request to the server. Upon arrival, the server communicates back with a `101 Switching Protocols` response.


## Unclassified

- [ ] Nest.js
- [ ] CloudFormation
- [ ] GraphQL
- [ ] Web Push
- [ ] Serverless Architecture
- [ ] Containerization
- [ ] TypeScript
- [ ] Microservices Architecture
- [ ] RESTful API
- [ ] Infrastructure as Code
- [ ] Continuous Integration
- [ ] Continuous Development
- [ ] RDBMS
- [ ] NoSQL
- [ ] Message Brokers
- [ ] Event-Driven Architecture
- [ ] Distributed Tracing: A method used to debug and monitor applications built using microservices architecture. Popular tools include Jaeger and Zipkin.
- [ ] ContentDelivery Network
- [ ] API Gateway
- [ ] Zero Downtime Deployments
- [ ] QA Automation
- [ ] Caching
- [ ] Cloud-Native Application Development
- [ ] Load Balancing
- [ ] Elasticity and Scalability in the Cloud
- [ ] Data Replication and Sharding
- [ ] Logging
- [ ] Monitoring
- [ ] Alerts
- [ ] Database Partitioning
- [ ] Real Time Streaming and Batch Processing
- [ ] Identity Provider
- [ ] Secrets Management
- [ ] Performance Tuning
- [ ] Stress Testing
- [ ] WebSockets and Real-Time Communication
- [ ] Deployment Strategies
- [ ] Git Submodule
- [ ] OAuth & OpenID Connect
- [ ] Stateless Architecture
- [ ] Web Application Firewall
- [ ] Reverse Proxy and Load Balancer
- [ ] HTTP Response Status Codes
- [ ] API Versioning
- [ ] Error Tracking and Exception Handling
- [ ] Messge Queues and Asynchronous Processing
- [ ] Microservices Observability: Communication between microservices can sometimes be complex and difficult to monitor. Tools like Istio and Linkerd provide the ability to visualize, control, and secure thr traffic between services.
- [ ] Feature Flagging: This development methodology can help make feature rollouts less risky and more steady. It enables developers to hid, enable or disable the feature in production, so they can safely test and release new features.
- [ ] Blud-Green Deployments
- [ ] Localization and Internationalization
- [ ] GraphQL Subscription
- [ ] CORS Configuration
- [ ] Rate Limiting and Throttling
- [ ] Unit Testing
- [ ] Integration Testing
- [ ] Dependency Injection
- [ ] End-toEnd Encryption
- [ ] Domain-Driven Design
- [ ] JSON Web Token
- [ ] Pagination
- [ ] Filtering
- [ ] Environment-Specific Configuration
- [ ] Scheduled Jobs and Cron Tasks
- [ ] Memory Management and Leaks Detection
- [ ] Two-Factor Authentication
- [ ] Service Mesh: A dedicated infrastructure layer for handling service-to-service communication, responsible for the reliable delivery of requests in a complex, networked system.
- [ ] Latency and Exception Monitoring
- [ ] API Design Principles
- [ ] gRPC
- [ ] Traffic Shadowing
- [ ] Health Checks and Self Healing System
- [ ] Test-Driven Development
- [ ] Circuit Breaker Design Pattern
- [ ] Event Sourcing: A technique that involves saving changes to application state as a sequence of events, which can be replayed to recreate the application state at any point in time.
- [ ] Command Query Responsibility Segregation (CQRS): This pattern separates read and update operations for a data store, optimizing for different needs of the two operations.
- [ ] IPV6 Transition
- [ ] WebRTC
- [ ] Distributed Caching
- [ ] HTTP/2 and HTTP/3
- [ ] HTTP Caching Strategy
- [ ] Server-Sent Event (SSE)
- [ ] Docker Compose
- [ ] Elastic STack
- [ ] GraphQL Federation
- [ ] Mutation Testing
- [ ] Runtime Type Checking
- [ ] Security Headers
- [ ] Server Timing Metrics: Metrics to measure where server time is spent while loading the application.
- [ ] Service Discovery: Enables automatic detection of services offered by a system.
- [ ] tRPC
