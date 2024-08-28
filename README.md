# Go Load Balancer

This project is a simple load balancer written in Go. It distributes incoming HTTP requests across multiple backend servers to ensure even load distribution and high availability.

## Features

Health Checks: Periodically checks the health of backend servers to ensure they are reachable.
Load Balancing: Distributes incoming requests to the next available backend server.

### Getting Started

#### Prerequisites

Go (version 1.16 or later)
Installation
Clone the repository:

### Build the project:

#### Usage

Run the load balancer with the following command:

-backends: Comma-separated list of backend servers.
-port: Port on which the load balancer will listen for incoming requests.
Example
This command starts the load balancer on port 3030 and distributes requests to http://localhost:8080 and http://localhost:8081.

## Health Checks

The load balancer performs health checks every 20 seconds to ensure that backend servers are reachable. If a backend server is not reachable, it will be temporarily removed from the pool of available servers.

License
This project is licensed under the MIT License. See the LICENSE file for details.
