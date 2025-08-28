# Microservices

Microservices architecture splits applications into smaller, independent services based on business functionalities. Each service is self-contained, developed, deployed, and scaled separately, enabling loose coupling and independent versioning.

## Monolithic Architecture

A monolithic architecture is a traditional model of a software program, which is built as a unified unit that is self-contained and independent from other applications. The word “monolith” is often attributed to something large and glacial, which isn’t far from the truth of a monolith architecture for software design.

A monolithic architecture is a singular, large computing network with one code base that couples all of the business concerns together. To make a change to this sort of application requires updating the entire stack by accessing the code base and building
and deploying an updated version of the service-side interface. This makes updates restrictive and time-consuming.

!!! danger "Challenges of Monolithic Architecture"
	- Application is too large and complex
	- Components are tightly coupled
	- Can only scale the entire app, not individual services
	- Difficulty managing different dependency versions
	- Longer release process
	- Every change requires testing and redeploying the whole application
	- Bugs in any module can bring down the entire app

## Microservices Benefits

!!! info "Why Microservices?"
	- Separation of concern: one service for one specific job
	- Independent development, deployment, and scaling
	- Loosely coupled services
	- Each microservice has its own version

## Communication Between Microservices

- **Synchronous (API calls):** Services communicate via HTTP requests and responses to API endpoints.
- **Asynchronous (Message Broker):** Services send messages to a broker (e.g., RabbitMQ), which forwards them to the target service.
- **Service Mesh:** External service (e.g., Istio, Consul) manages communication logic, offloading it from microservices.

!!! note "Distributed System Challenges"
	- Configuring communication between services (handling downtime, retries)
	- Monitoring multiple instances across servers
	- Added complexity due to distribution
	- Tools: Messaging, Service Mesh, Monitoring, Security, Containers, Orchestration

## Monorepo vs Polyrepo

### Monorepo (Single Repository)

!!! success "Monorepo Advantages"
	- One Git repository for all projects/services
	- Easier code management and development
	- Shared code and configuration
	- Changes tracked, tested, and released together

!!! danger "Monorepo Challenges"
	- Tight coupling of projects
	- Large codebase slows git operations
	- Additional logic needed for selective builds/deploys
	- Issues can affect all projects/teams

### Polyrepo (Multiple Repositories)

!!! success "Polyrepo Advantages"
	- One repository per service
	- Code is isolated; work on each service separately
	- Better access control and isolation
	- Each repository has its own pipeline

!!! danger "Polyrepo Challenges"
	- Cross-cutting changes are harder
	- Changes across projects require separate merge requests
	- Tedious switching between projects
	- More difficult searching, testing, debugging, and sharing resources

**General rule:** Use monorepo for smaller microservice applications; use polyrepo for separate teams, better isolation, and independent pipelines.

## Best Practices for Managing Microservices
- **Single-Responsibility Principle (SRP):** Each module or microservice should have only one function. SRP and continuous integration (CI) automate code quality checks before merging, improving velocity and reducing the need for separate QA. CI precedes continuous delivery (CD), which keeps software ready to deploy.
- **API Gateways:** Simplify communication between microservices, manage authentication and authorization, and boost security.
- **Asynchronous Communication:** Preserves autonomy and reduces dependencies that might slow application function.
- **Versioning Microservices:** Critical when implementing breaking changes (e.g., removing an operation). Versioning smooths transitions and minimizes service disruption.
