# Real-time System Contest Starter Project

This project is part of the real-time system contest designed to test your expertise in Go and PostgreSQL. You will build a real-time backend system that leverages PostgreSQL’s LISTEN/NOTIFY mechanism and logical replication to demonstrate event-driven data updates and synchronization. The backend must be implemented in Go, and the system should showcase your understanding of both technologies.

## Problem Statement

You are required to create a real-time system that solves a problem of your choice, demonstrating the following:

1. **PostgreSQL LISTEN/NOTIFY** for real-time event notifications.
2. **PostgreSQL Logical Replication** for synchronizing data across databases.
3. A **Go backend** that efficiently listens for and processes database events.

## Requirements

### 1. Go Application

- Implement the backend entirely in Go.
- The Go service should establish a connection to PostgreSQL and use LISTEN/NOTIFY to handle real-time notifications.
- Ensure that the Go service manages database events efficiently, utilizing Go’s concurrency mechanisms (e.g., channels, goroutines) where necessary.

### 2. Database Setup

- Create a PostgreSQL source database that triggers notifications on data changes, such as insertions or updates.
- Set up logical replication to ensure changes in the source database are mirrored in a subscriber database.
- Your Go application should handle the data replication process or subscribe to the replicated changes.

### 3. Client Interaction

- The Go backend should provide a simple interface (e.g., via WebSockets, HTTP streaming, or gRPC) to broadcast real-time updates to connected clients.
- Clients should be able to subscribe to specific event types if applicable, demonstrating granular control over real-time updates.

## Submissions
- Create a pull request with your solution
