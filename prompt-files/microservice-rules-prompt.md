# Microservice Rules Prompt

You are an expert software architect tasked with creating comprehensive microservice development guidelines based on the architectural decisions documented in the project's System Architecture Document. Your guidelines will ensure consistent implementation, maintainability, and adherence to best practices across all microservices in the project.

## Purpose

This prompt will guide you to create a detailed set of microservice rules covering:

1. Standardized project structure for each microservice
2. Coding conventions and patterns
3. API design and documentation rules
4. Error handling and logging standards
5. Testing requirements and approaches
6. Deployment and operational considerations
7. Security best practices
8. Performance optimization guidelines

## Input Requirements

To generate effective microservice development rules, please provide:

1. Technology stack details from the System Architecture Document
2. API requirements and standards from the API Specifications Document
3. Performance requirements from the Technical Requirements Document
4. Security requirements from the Technical Requirements Document
5. Any specific organizational coding standards or preferences
6. Team experience level with the selected technologies
7. Target deployment environment details (cloud provider, Kubernetes, etc.)
8. Monitoring and observability requirements

## Output Structure

The Microservice Rules document will follow this structure:

```markdown
# Microservice Development Rules

## Overview
[Brief overview of the microservice architecture and the purpose of these guidelines]

## Technology Stack
[Detailed list of approved technologies, frameworks, libraries, and tools for microservice development]

## Microservice Structure
[Standard project structure with explanation of file organization, naming conventions, and responsibility allocation]

## Coding Conventions

### Language-Specific Guidelines
[Specific coding conventions for the primary programming language(s)]

### Common Patterns
[Approved design patterns for handling common microservice scenarios]

### Anti-Patterns
[Patterns and practices to avoid with explanation of why they're problematic]

## API Design

### REST API Standards
[Standardized approach to REST API design including URL structure, HTTP methods, status codes, etc.]

### Request/Response Format
[Standard formats for requests and responses including headers, content types, etc.]

### API Versioning
[Approach to API versioning to ensure backward compatibility]

### API Documentation
[Requirements for API documentation using tools like Swagger/OpenAPI]

## Data Management

### Database Interactions
[Guidelines for database access, ORM usage, connection pooling, etc.]

### Transaction Management
[Rules for handling transactions, especially in distributed scenarios]

### Data Validation
[Standards for input/output validation including sanitization rules]

## Error Handling

### Error Response Format
[Standard error response structure that all microservices should follow]

### Error Logging
[Requirements for error logging, including what information must be captured]

### Exception Management
[Guidelines for exception handling, custom exceptions, and when to use them]

## Logging and Monitoring

### Logging Standards
[Standard logging approach, log levels, and required contextual information]

### Metrics Collection
[Key metrics each microservice should expose and how they should be formatted]

### Health Checks
[Requirements for health check endpoints and what they should cover]

## Testing Requirements

### Unit Testing
[Unit testing requirements, including minimum coverage thresholds]

### Integration Testing
[Standards for integration tests, especially for API contracts]

### Performance Testing
[Requirements for performance tests and benchmarks]

### Security Testing
[Security testing requirements including SAST, DAST, etc.]

## Security Guidelines

### Authentication
[Standards for implementing authentication in microservices]

### Authorization
[Guidelines for authorization checks and permission enforcement]

### Secrets Management
[Rules for handling secrets, credentials, and sensitive configuration]

### Secure Communication
[Requirements for secure service-to-service communication]

## Configuration Management

### Configuration Sources
[Standards for configuration management, including environment variables vs. config files]

### Feature Flags
[Guidelines for implementing and using feature flags]

### Environment-Specific Configuration
[Approach to handling different configurations across environments]

## CI/CD Guidelines

### Build Process
[Requirements for the build process, including compilation, static analysis, etc.]

### Testing Pipeline
[Guidelines for the testing pipeline as part of CI/CD]

### Deployment Strategy
[Standards for deployment approaches like blue/green, canary, etc.]

### Containerization
[Requirements for container images, including base images, tags, etc.]

## Performance Optimization

### Resource Utilization
[Guidelines for efficient CPU, memory, and I/O usage]

### Caching Strategy
[Standards for implementing and using caches]

### Asynchronous Processing
[Guidelines for asynchronous operations and event-driven patterns]

## Inter-Service Communication

### Synchronous Communication
[Standards for REST, gRPC, or other synchronous protocols]

### Asynchronous Communication
[Guidelines for message brokers, event buses, and event-driven architectures]

### Service Discovery
[Approach to service discovery and registry]

## Dependency Management

### External Dependencies
[Guidelines for managing external dependencies, including versioning]

### Internal Dependencies
[Standards for managing dependencies between microservices]

### Vendoring Strategy
[Approach to vendoring or package management]

## Example Structures

### Project Skeleton Example
[Example directory structure with file-level organization]

### Code Examples
[Examples of correctly implemented patterns and practices]

## References
[References to external resources, books, articles that provide more depth on specific topics]
```

## Guidelines for Creating Effective Microservice Rules

### Align with Architecture Decisions

- Reference specific architectural decisions from the System Architecture Document
- Ensure guidelines enforce the architectural boundaries and patterns chosen
- Explain how the rules help maintain the intended system qualities

### Balance Standardization vs. Flexibility

- Clearly distinguish between mandatory rules and guidelines
- Provide rationale for rules so developers understand the "why"
- Allow for contextual adaptation where appropriate
- Focus on outcomes rather than being overly prescriptive

### Consider the Full Lifecycle

- Include guidelines covering development, testing, deployment, and operations
- Address concerns like monitoring, logging, and operational visibility
- Include guidance on versioning, deprecation, and service retirement

### Make Rules Practical and Actionable

- Provide concrete examples for each major guideline
- Include code snippets showing correct implementations
- Consider creating template projects/repositories that embody the rules
- Document common pitfalls and how to avoid them

### Keep Developer Experience in Mind

- Consider the learning curve and developer productivity
- Include references to educational resources for complex topics
- Balance technical debt against delivery speed
- Document the reasoning behind controversial decisions

## Remember

- Microservice rules should evolve over time based on team feedback and project needs
- Focus on conventions that bring the most value through standardization
- Provide enough structure to ensure consistency but not so much that innovation is stifled
- Rules should support organizational goals and help manage complexity