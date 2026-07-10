# Zinnia

## What it is
Zinnia is a full-stack HPC (high-performance computing) cluster operations dashboard built with ASP.NET Core and React. It simulates a computing cluster by tracking nodes, jobs, failures, and utilization metrics while providing live updates through a web dashboard.

The project was built to demonstrate backend API development, real-time communication, database modeling, and containerized deployment.

### Why it is
I became intersted in HPC upon reading articles about the Lawrence Livermore National Laboratory and its mission of securing the U.S. nuclear deterrent.

Lawrence Livermore National Laboratory is the home of the El Capitan supercomputer, which allows scientists to simulate complex physics. El Capitan is the world's second-fastest computer.

## Features
- Simulated HPC cluster with compute nodes and job scheduling
- Live dashboard updates using SignalR
- Job lifecycle management (Pending, Running, Completed, Failed)
- Cluster health and utilization monitoring
- ASP.NET Core Web API with Entity Framework Core and SQL Server
- React frontend for real-time visualization
- Docker support for local deployment

## Tech stack
- C#
- ASP.NET Core Web API
- Entity Framework Core
- SQL Server
- SignalR
- React
- Docker

## Get started

### Prerequisites
- .NET SDK
- Node.js
- SQL Server
- Docker <small>(for containerized deployment; optional)</small>

### Running the project
Clone the repository:
- `git clone https://github.com/marljonson/zinnia.git`
- `cd zinnia`
Run the backend:
- `cd backend`
- `dotnet restore`
- `dotnet run`
Run the frontend:
- `cd frontend`
- `npm install`
- `npm start`
Or start the full application with Docker:
- `docker compose up --build`

## Project overview
The backend simulates an HPC cluster by generating node activity, scheduling jobs, tracking state transitions, and explosing cluster data through a REST API and SignalR hub.

The React frontend subscribes to real-time updates to display node status, job queues, active workloads, failures, and utilization metrics.

## Future improvements
- Configurable scheduling algorithms (FIFO, Priority, Round Robin)
- Historical metrics and trend charts
- User authentication and role-based access
- Job subission and cancelation from the dashboard
- Multi-cluster simulation support
