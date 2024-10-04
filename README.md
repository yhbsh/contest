Contest Task: Build a Real-time System Using PostgreSQL Publish/Notify and Logical Replication in Go

Overview:

This contest is designed to test your expertise in both Go and PostgreSQL. You will build a real-time backend system that leverages PostgreSQL’s LISTEN/NOTIFY mechanism and logical replication for event-driven data updates and synchronization. The backend must be implemented in Go, and the system should demonstrate your understanding of both technologies.

Problem Statement:

Create a real-time system that solves a problem of your choice, demonstrating:

1. PostgreSQL LISTEN/NOTIFY for real-time event notifications.


2. PostgreSQL Logical Replication for synchronizing data across databases.


3. Go backend that listens for events and processes them efficiently.



Requirements:

1. Go Application:

Implement the backend entirely in Go.

The Go service should establish connections to PostgreSQL and use LISTEN/NOTIFY to handle real-time notifications.

Ensure that the Go service manages database events efficiently, using channels, goroutines, or other concurrency patterns where necessary.



2. Database Setup:

Create a PostgreSQL source database that triggers notifications on data changes (e.g., on insert or update).

Set up a logical replication to ensure changes in the source database are mirrored in a subscriber database.

Your Go application should handle the data replication process or subscribe to the replicated changes.



3. Client Interaction:

The Go backend should provide a simple interface (e.g., via WebSockets, HTTP streaming, or gRPC) to broadcast real-time updates to connected clients.

Clients should be able to subscribe to specific event types, if applicable, to demonstrate granular control over real-time updates.



4. Submission Details:

Write clear instructions on how to set up the system locally, including PostgreSQL and Go.

Provide a minimal Go client that listens for real-time events, or show how to use tools like curl or a WebSocket client to connect to your system.

Your code should be clean, modular, and follow Go best practices for error handling and concurrency management.




Instructions for Submission:

1. Fork this repository which contains basic PostgreSQL and Go setup instructions.


2. Complete the solution and push the code to your fork.


3. In the README.md, provide:

Setup instructions for PostgreSQL and logical replication configuration.

How to run the Go service and test real-time updates.

Steps to validate that both the notification system and replication work as expected.



4. Submit the GitHub repo link via the submission form [link to form].


5. Your code must be well-documented and written for maintainability and production-readiness.



Judging Criteria:

Proficiency in Go and PostgreSQL: Your ability to write Go code that interacts with PostgreSQL effectively.

Concurrency Handling: Use of Go’s concurrency patterns (goroutines, channels) to handle database events and real-time communication.

Performance and Scalability: Ability to handle multiple concurrent clients or events without performance degradation.

Correctness: Proper use of PostgreSQL LISTEN/NOTIFY and logical replication to create a real-time system.

Documentation: Clear setup instructions and well-commented code.


Bonus Points:

Use advanced Go patterns such as context management, error propagation, and custom middleware.

Implement a client in Go that can interact with the backend over WebSockets or gRPC.

Demonstrate optimizations for performance, such as batching notifications or connection pooling.



---

This contest will evaluate your ability to build robust real-time systems using Go and PostgreSQL, focusing on your mastery of concurrency and database interaction.
