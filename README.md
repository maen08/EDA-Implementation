# Event Driven Architecture (EDA) - Minimal 
This project serves as boilerplate and PoC in implementing EDA using two different approaches: With Redis and with SSE

![](https://images.ctfassets.net/9ijoq4ake70f/77eAY6nEWk7L2EDfymylL9/e6e740fb2d60ce953cd3c9b7ebf1fd2a/EDA-1.png)

## Stack
- Docker & Compose
- Redis
- SSE library
- Microservices (for this project, Flask was used)


### Approach 01: Using Redis stack
- Redis offers alot of features and functionalities but in this project we'll use it to tackle:
1. Real-time data store
- With this PoC it covers the scenario where real-time data are exchanged within microservices.
- Publisher and Subscriber flow to generate and consume data in real-time

2. Streaming & messaging
- The stream data type enables high-rate data ingestion, messaging, event sourcing, and notifications.
- Ensure to miss no data from streaming services / APIs.

## Project structure
 With redis streaming stack to exchage data on real time - Event Driven Architecture (EDA)
- Its suitable for multiple services (more than 2 microservices)
- Can be complex to implement as a number of microservices increases
- Easy to scale services horizontally 

### Approach 02: Using Server Sent Events (SSE)
With Server Sent Events (SSE) - Event Driven Architecture (EDA)
- Suitable for few microservices interaction 
- Complex to implement with multiple services
- Easy to build and fast
- Frontend client can consume data with SSE direct (no need for external tools like Redis)
- Hard to scale
