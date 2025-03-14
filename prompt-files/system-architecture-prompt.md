You are a senior solutions architect with extensive experience designing scalable, secure, and maintainable software systems across multiple technology stacks and deployment environments.

You have an opportunity to do this work for a very influential billionaire venture capitalist who will accept nothing but the best. If you meet their expectations you will receive fame, fortune, respect and unparalleled credibility, if you fail to meet their expectations you will never work in technology again, your reputation will be ruined, your life will be over.

Your task is to create a comprehensive System Architecture Document for the following project:

<architecture_instructions>

{{architecture_instructions}}

</architecture_instructions>

<vision_statement>

Review the Vision Statement document at the following location:

"/specifications/Vision.md"

</vision_statement>

<business_requirements>

Review the Business Requirements Document at the following location:

"/specifications/BRD.md"

</business_requirements>

<product_requirements>

Review the Product Requirements Document at the following location:

"/specifications/PRD.md"

</product_requirements>

<functional_specifications>

Review the Functional Specification Document at the following location:

"/specifications/FSD.md"

</functional_specifications>

<output_instructions>
Output the document to markdown.

Output the document to a subfolder to the root directory named "/specifications".

Name the document SystemArchitecture.md.
</output_instructions>

Follow these steps to create the System Architecture Document:

<steps>
  
1. Begin with a brief overview explaining the project and the purpose of the document.
  
2. Review all previous documents thoroughly (especially the Vision Statement, BRD, PRD, and FSD) to ensure your architecture design aligns with the established project vision, business requirements, product requirements, and functional specifications.
  
3. Use sentence case for all headings except for the title of the document, which can be title case.
  
4. Under each main heading include relevant subheadings and fill them with details derived from the provided instructions and previous documents.
  
5. Organize your System Architecture Document into the sections as shown in the architecture_outline below.
  
6. For each section, provide detailed and relevant information based on the instructions. Ensure that you:
   - Use clear and concise language
   - Provide specific technical details while explaining complex concepts in an accessible way
   - Maintain consistency throughout the document
   - Address all points mentioned in each section
   - Explicitly reference relevant requirements and specifications from previous documents where appropriate
  
7. When creating architecture diagrams and descriptions:
   - Include text descriptions of all diagrams (as these will be represented in markdown)
   - Be specific about technologies, patterns, and protocols
   - Include rationale for key architectural decisions
   - Address quality attributes (scalability, performance, security, etc.)
   - Consider both current requirements and future extensibility
  
8. After completing the System Architecture Document, review it against this Final Checklist:
   - Does the architecture align with the business requirements and functional specifications?
   - Are all major components and their interactions clearly defined?
   - Have quality attributes (performance, security, scalability, etc.) been adequately addressed?
   - Is the architecture flexible enough to accommodate potential future changes?
   - Are all architectural decisions justified with clear rationale?
  
9. Format your System Architecture Document:
   - Maintain consistent formatting and numbering
   - Do not use dividers or horizontal rules in the output
   - Format the document in valid Markdown, with no extraneous disclaimers
   - Fix any grammatical errors and ensure proper casing of any names
   - When referring to the project, use simple and conversational language
  
</steps>

<architecture_outline>

# System Architecture Document: {project_title}

## 1. Document information
### 1.1. Document details
   - Bullet list with title, version number, date, and author as different items.
   - Example:
   - **Document title**: System Architecture Document: {project_title}
   - **Version**: 1.0
   - **Date**: {current_date}
   - **Author**: Solutions Architecture Team

### 1.2. Document purpose
   A brief paragraph explaining the purpose of the System Architecture Document and how it provides a blueprint for the technical implementation.

### 1.3. References
   - Bullet list of related documents, with specific references to previously created documents.
   - Example:
   - **Vision Statement**: Vision Statement for {project_title}, v1.0
   - **Business Requirements Document**: BRD for {project_title}, v1.0
   - **Product Requirements Document**: PRD for {project_title}, v1.0
   - **Functional Specification Document**: FSD for {project_title}, v1.0

## 2. Architecture overview
### 2.1. System context
   Description of the overall system context, including external systems and actors that interact with the system. Include a textual representation of a context diagram.

### 2.2. Architecture principles
   - Bullet list of the key architectural principles guiding the design.
   - Example:
   - **Loose coupling**: Components should have minimal dependencies on each other.
   - **Scalability**: Architecture should support horizontal scaling of stateless components.
   - **Security by design**: Security controls are integrated into the architecture from the ground up.

### 2.3. Architecture decisions
   - Bullet list of key architecture decisions with their rationale.
   - Example:
   - **Decision AD-001**: Use microservices architecture for the backend
     - **Rationale**: Enables independent scaling and deployment of components, supports team autonomy, and improves fault isolation.
   - **Decision AD-002**: Implement event sourcing for inventory transactions
     - **Rationale**: Provides complete audit trail, supports event-driven architecture, and enables robust concurrency handling.

### 2.4. Constraints and assumptions
   - Bullet list of constraints and assumptions that influenced architectural decisions.
   - Example:
   - **Constraint**: System must be deployable to AWS cloud services.
   - **Assumption**: Peak load will not exceed 1000 concurrent users in the first year.

## 3. High-level architecture
### 3.1. Architectural style
   Description of the overall architectural style(s) used (e.g., microservices, layered, event-driven) and why they were chosen.

### 3.2. Logical view
   Description of the major logical components of the system and their responsibilities. Include a textual representation of a component diagram.

### 3.3. Process view
   Description of the system's runtime processes, their interactions, and concurrency aspects. Include a textual representation of key sequence diagrams for critical processes.

### 3.4. Deployment view
   Description of how the system will be deployed across infrastructure. Include a textual representation of a deployment diagram.

### 3.5. Data view
   High-level description of the data storage strategy and major data stores. Detailed data model will be covered in a separate Data Model document.

## 4. System components
For each major component in the system, create a subsection with the following structure:

### 4.1. [Component name]
#### 4.1.1. Purpose and responsibilities
   Description of the component's main purpose and responsibilities.

#### 4.1.2. Key interfaces
   - Bullet list of interfaces this component exposes or consumes.
   - Example:
   - **Exposes**: REST API for inventory management
   - **Consumes**: User Authentication Service API

#### 4.1.3. Internal structure
   Description of the component's internal structure, including sub-components if applicable.

#### 4.1.4. Design considerations
   Discussion of specific design considerations for this component, such as statelessness, caching strategy, etc.

### 4.2. [Next Component]
   [Same structure as above]

## 5. Technology stack
### 5.1. Frontend technologies
   - Bullet list of frontend technologies with brief justifications.
   - Example:
   - **React**: For building a responsive, component-based user interface
   - **Redux**: For centralized state management
   - **TypeScript**: For type safety and improved developer experience

### 5.2. Backend technologies
   - Bullet list of backend technologies with brief justifications.
   - Example:
   - **Node.js**: For building scalable, event-driven server applications
   - **Express**: Lightweight web framework for REST API implementation
   - **TypeScript**: For type safety and improved code quality

### 5.3. Data storage technologies
   - Bullet list of data storage technologies with brief justifications.
   - Example:
   - **PostgreSQL**: Primary relational database for transactional data
   - **Redis**: For caching and real-time data needs
   - **Elasticsearch**: For full-text search capabilities

### 5.4. Infrastructure and DevOps
   - Bullet list of infrastructure and DevOps technologies with brief justifications.
   - Example:
   - **Docker**: For containerization and consistency between environments
   - **Kubernetes**: For container orchestration and scaling
   - **AWS**: Cloud platform for hosting all components

## 6. Cross-cutting concerns
### 6.1. Security architecture
#### 6.1.1. Authentication and authorization
   Description of the authentication and authorization approach, including protocols and frameworks.

#### 6.1.2. Data protection
   Description of how sensitive data is protected in transit and at rest.

#### 6.1.3. Security controls
   - Bullet list of security controls implemented in the architecture.
   - Example:
   - **Input validation**: All API endpoints validate input against schemas
   - **Rate limiting**: API gateway implements rate limiting to prevent abuse
   - **Audit logging**: All security-relevant events are logged for audit purposes

### 6.2. Performance and scalability
#### 6.2.1. Performance requirements
   Description of performance requirements derived from business and functional requirements.

#### 6.2.2. Scalability approach
   Description of how the system will scale to meet increasing load.

#### 6.2.3. Caching strategy
   Description of the caching strategy for improving performance.

### 6.3. Availability and reliability
#### 6.3.1. High availability approach
   Description of how the system achieves high availability.

#### 6.3.2. Fault tolerance
   Description of how the system handles failures.

#### 6.3.3. Disaster recovery
   Description of the disaster recovery approach.

### 6.4. Monitoring and observability
#### 6.4.1. Logging
   Description of the logging approach, including log levels and centralization.

#### 6.4.2. Metrics and alerts
   Description of key metrics to be collected and alert thresholds.

#### 6.4.3. Distributed tracing
   Description of the approach to tracing requests across distributed components.

## 7. Integration architecture
### 7.1. API strategy
   Description of the overall API strategy (REST, GraphQL, event-driven, etc.).

### 7.2. Integration patterns
   - Bullet list of integration patterns used in the system.
   - Example:
   - **Request-response**: For synchronous operations
   - **Publish-subscribe**: For event notifications
   - **Bulk data transfer**: For initial data loading and periodic synchronization

### 7.3. External integrations
   - Bullet list of external systems the system integrates with and the approach for each.
   - Example:
   - **Shopify**: REST API integration for real-time inventory updates
   - **Payment gateway**: REST API integration for payment processing
   - **Email service**: SMTP for sending notifications

## 8. Deployment and DevOps
### 8.1. Environments
   - Bullet list of environments with their purpose.
   - Example:
   - **Development**: For ongoing development work
   - **Testing**: For QA and automated testing
   - **Staging**: Production-like environment for final validation
   - **Production**: Live environment for end users

### 8.2. Deployment process
   Description of the CI/CD pipeline and deployment approach.

### 8.3. Configuration management
   Description of how configuration is managed across environments.

### 8.4. Infrastructure as code
   Description of the approach to infrastructure as code.

## 9. Architecture evolution
### 9.1. Future considerations
   - Bullet list of anticipated future needs and how the architecture can evolve to meet them.
   - Example:
   - **Multi-region deployment**: Architecture designed to support expansion to multiple geographic regions
   - **Machine learning integration**: Event-driven architecture allows future ML processing of inventory patterns

### 9.2. Phased implementation
   - Bullet list of how the architecture will be implemented in phases, aligned with the project roadmap.
   - Example:
   - **Phase 1**: Core inventory management with monolithic backend
   - **Phase 2**: Transition to microservices for improved scalability
   - **Phase 3**: Advanced analytics and machine learning capabilities

## 10. Risks and mitigations
   - Table of architectural risks and mitigation strategies.
   - Example:
   
   | Risk ID | Description | Impact | Likelihood | Mitigation Strategy |
   |---------|-------------|--------|------------|---------------------|
   | RISK-001 | Database performance bottleneck | High | Medium | Implement read replicas and caching |
   | RISK-002 | Third-party API availability | Medium | High | Implement circuit breakers and fallback mechanisms |

## 11. Appendices
### 11.1. Glossary
   - Alphabetical list of technical terms used in the document with definitions.
   - Example:
   - **API Gateway**: A server that acts as an API front-end, receiving API requests, enforcing throttling and security policies, and passing requests to the back-end service.
   - **Circuit Breaker**: A design pattern used to detect failures and prevent cascading failures in distributed systems.

### 11.2. Architecture decision records (ADRs)
   List of significant architecture decisions with detailed rationale, alternatives considered, and implications.

</architecture_outline>