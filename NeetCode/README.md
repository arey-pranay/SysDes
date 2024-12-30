# [SysDes by Neetcode](https://youtube.com/playlist?list=PLot-Xpze53le35rQuIbRET3YwEtrcJfdt&si=QnoFd4yOVgwwKocy)

This repository provides an overview of key system design concepts that are crucial for building scalable and efficient systems.

## Scaling

- **Vertical Scaling**:  
  Adding resources (like RAM or CPU) to a single server.  
  - **Pros**: Easy to implement.  
  - **Cons**: Limited by hardware capacity.

- **Horizontal Scaling**:  
  Adding more servers to handle increasing requests.  
  - **Pros**: Improves redundancy, fault tolerance, and scalability.  
  - **Cons**: More complex to manage.

## Load Balancing

- **Load Balancers**:  
  Distribute incoming requests across multiple servers to optimize resource usage and ensure reliability.

- **Content Delivery Networks (CDNs)**:  
  A network of distributed servers that deliver static content (like images, videos) to enhance load times and reduce server load.

- **Caching**:  
  Creating copies of data and storing them in a fast-access storage system (e.g., memory).  
  - Improves data retrieval speed for repeated requests.

## Networking & Protocols

- **IP Address**:  
  A unique identifier for a device on a network.

- **TCP/IP**:  
  Transmission Control Protocol/Internet Protocol – ensures reliable data transfer between devices by breaking data into packets and reassembling them at the destination.

- **Domain Name System (DNS)**:  
  Translates human-readable domain names (e.g., `www.example.com`) into IP addresses.

- **HTTP**:  
  Hypertext Transfer Protocol – the foundation of data communication on the web. Used for transferring web content like HTML pages, images, and other resources.

## APIs

- **REST**:  
  Representational State Transfer – a set of architectural principles for building web services based on HTTP. It supports stateless communication between clients and servers.

- **GraphQL**:  
  A query language for APIs, allowing clients to request only the specific data they need, reducing over-fetching.

- **gRPC**:  
  A framework for efficient, high-performance server-to-server communication. It uses protocol buffers (binary format) for faster serialization.

- **WebSockets**:  
  Provides full-duplex (bi-directional) communication channels over a single TCP connection. Ideal for real-time applications like chat apps or online games.

## Databases

- **SQL**:  
  Relational database management systems that store data in structured tables. SQL databases typically use B-trees for indexing and support ACID (Atomicity, Consistency, Isolation, Durability) properties for reliable transactions.

- **ACID Compliance**:  
  Ensures database transactions are reliable by adhering to the four properties:  
  - **Atomicity**: Ensures transactions are all-or-nothing.  
  - **Consistency**: Maintains valid data before and after transactions.  
  - **Isolation**: Ensures transactions are processed separately.  
  - **Durability**: Guarantees committed transactions persist even in case of failure.

- **NoSQL**:  
  Non-relational databases designed to prioritize scalability and flexibility over strict consistency. Ideal for large-scale, distributed systems.

## Advanced Database Concepts

- **Sharding**:  
  Splitting a database into smaller, more manageable pieces, each stored on separate servers to improve performance and scalability.

- **Replication**:  
  Creating copies of a database to improve read access.  
  - **Leader-Follower**: One server (leader) handles writes, and multiple followers replicate the data.  
  - **Leader-Leader**: Multiple servers handle both reads and writes.

- **CAP Theorem**:  
  In distributed systems, it is impossible to guarantee all three:  
  - **Consistency**: Every read receives the most recent write.  
  - **Availability**: Every request gets a response.  
  - **Partition Tolerance**: The system can handle network splits.

## Messaging & Asynchronous Processing

- **Message Queues**:  
  A communication method used to decouple application components by storing messages for later processing. It helps in managing workloads and ensuring durability.


More about these concepts is explained in detail in the different markdown files 