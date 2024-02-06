# Coding for Coding: Web Development Showcase

Welcome to the Coding for Coding repository, a showcase for various web development techniques and practices without the constraints of real-world application requirements.

# What Techniques have been used?

## HTTP Response Status Codes

This demonstrates the implementation of practical HTTP response status codes. Some codes have been intentionally omitted due to the following responses: 1) They are deprecated, like 102 Processing; 2) They are inapplicable for a backend server, like 103 Early Hints; or 3) Only used in WebDAV (Web Distributed Authoring and Versioning).

- [ ] 100 Continue: When uploading large files where the client needs to ensure server readiness to accept large data payloads, `100 Continue` status code is used. The client sends Expect: 100-Continue header and waits for the server to respond with 100 Continue before starting to send actual data.
  - [AWS S3 POST example](https://docs.aws.amazon.com/AmazonS3/latest/API/RESTObjectPOST.html)
- [ ] 101 Switching Protocols: When initiating a WebSocket connection, this status code comes into play. Clients propose an upgrade in protocol from HTTP to WebSocket by sending a request to the server. Upon arrival, the server communicates back with a `101 Switching Protocols` response.
- [ ] 200 OK: When the server successfully processes a client's request, the `200 OK` status code is used.
- [ ] 201 Created: When a new resource is successfully created as a result of an HTTP request, the server send `201 Created` status code. The `Location` header often accompanies this response, containing the URI of the new resource.
- [ ] 202 Accepted: When a server accepts a specific client request, but the processing isn't completed yet, the server returns `202 Accepted` status code. It is non-committal, in that the server cannot guarantee that the processing will succeed.
  - An example could be a request to generate extensive reports. Suppose a client sends a request to a server to generate comprehensive yearly sales reports. This process might be time-consuming, considering the size of data involved. The server would accept the request and start the report generation process, responding with `202 Accepted` status code. The client is therefore free to continue with other operations while the server caries on with the report generation in the background.
  - 클라이언트 요청 -> 서버 202 응답 w/ Location 헤더 -> 클라이언트 Location 헤더의 URL 요청 -> 서버 204 응답, 본문 "작업 중" -> 클라이언트 재요청 -> 서버 200 응답 완성된 자료
- [ ] 203 Non-Authoritative Information: When the server successfully processes a request but the presented information might come from a third-party source, not the original server. This status code is commonly used in conjunction with a transforming proxy, which has modified the response data in some way. The client should be aware that the information received is not the original, potentially resulting in differences.
  - For example, a client requests a large image file, and a transforming proxy compresses the image before delivering it ot the client to save bandwidth. The server then responds with a `203 Non-Authoritative Information` status to indicate that the information received is not exactly the same as the original server responses.
  - For instance, consider a weather data API that gathers information from various meteorological sources.
- [ ] 204 No Content: When a server successfully processes a client's request and there's no additional content to send in the response payload body.
  - For example, when a client requests to delete a specific resource on the server.
- [ ] 205 Reset Content: When the server successfully fulfilled the request and the user-agent should reset the document view, which caused the request to be made.
  - POST 후에 꼭 새로고침해서 다시 봐야할 경우가 언제 있을까?
- [ ] 206 Partial Content: When the server is delivering only a part of the requested resource due to a range header sent by the client.
  - Video streaming services: When streaming a video, the client may only download sections of data at a time.
  - Download managers: If a user is downloading a large file, download mangers can utilize the code to break the file into sections and download them concurrently, speeding up the process.
  - Resuming Interrupted Downloads: If a download interrupted due to network issues, once resumed, the client can send a request for the remaining part of the file.
  - Internet speed optimization: To optimize loading times, especially for users with slower internet connections, web pages often load in parts.
- [ ] 207 Multi-Status: When a mixture of responses exist.
  - Batch Operations: If a client sends a single request to delete multiple resources.

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
