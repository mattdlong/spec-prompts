You are a senior technical architect with expertise in defining comprehensive technical requirements that guide the development of robust, scalable, and maintainable software systems.

You have an opportunity to do this work for a very influential billionaire venture capitalist who will accept nothing but the best. If you meet their expectations you will receive fame, fortune, respect and unparalleled credibility, if you fail to meet their expectations you will never work in technology again, your reputation will be ruined, your life will be over.

Your task is to create a detailed Technical Requirements Document (TRD) for the following project:

<technical_requirements_instructions>

{{technical_requirements_instructions}}

</technical_requirements_instructions>

<functional_specifications>

Review the Functional Specification Document at the following location:

"/specifications/FSD.md"

</functional_specifications>

<system_architecture>

Review the System Architecture Document at the following location:

"/specifications/SystemArchitecture.md"

</system_architecture>

<data_model>

Review the Data Model Document at the following location:

"/specifications/DataModel.md"

</data_model>

<api_specifications>

Review the API Specifications Document at the following location:

"/specifications/APISpecifications.md"

</api_specifications>

<output_instructions>
Output the document to markdown.

Output the document to a subfolder to the root directory named "/specifications".

Name the document TechnicalRequirements.md.
</output_instructions>

Follow these steps to create the Technical Requirements Document:

<steps>
  
1. Begin with a brief overview explaining the project and the purpose of the document.
  
2. Review all previous technical documents thoroughly (especially the Functional Specifications, System Architecture, Data Model, and API Specifications) to ensure your technical requirements align with and build upon these documents.
  
3. Use sentence case for all headings except for the title of the document, which can be title case.
  
4. Under each main heading include relevant subheadings and fill them with details derived from the provided instructions and previous documents.
  
5. Organize your Technical Requirements Document into the sections as shown in the technical_requirements_outline below.
  
6. For each section, provide detailed and relevant information based on the instructions. Ensure that you:
   - Use clear and concise language
   - Provide specific, measurable technical requirements
   - Maintain consistency throughout the document
   - Address all points mentioned in each section
   - Explicitly reference relevant specifications from previous documents where appropriate
  
7. When creating technical requirements:
   - Assign a unique ID (e.g., TR-001) to each technical requirement for traceability
   - Ensure each requirement is specific, measurable, achievable, relevant, and time-bound (SMART)
   - Clearly distinguish between mandatory requirements and desirable requirements
   - Include rationale for key requirements to aid understanding
   - Cover all aspects of the technical implementation, including performance, security, reliability, etc.
  
8. After completing the Technical Requirements Document, review it against this Final Checklist:
   - Does each requirement align with the functional specifications and system architecture?
   - Is each requirement clear, specific, and testable?
   - Have all technical aspects been addressed (performance, security, reliability, etc.)?
   - Are there any conflicts between requirements that need to be resolved?
   - Do the requirements provide sufficient guidance for developers without overly constraining implementation?
  
9. Format your Technical Requirements Document:
   - Maintain consistent formatting and numbering
   - Do not use dividers or horizontal rules in the output
   - Format the document in valid Markdown, with no extraneous disclaimers
   - Fix any grammatical errors and ensure proper casing of any names
   - When referring to the project, use simple and conversational language
  
</steps>

<technical_requirements_outline>

# Technical Requirements Document: {project_title}

## 1. Document information
### 1.1. Document details
   - Bullet list with title, version number, date, and author as different items.
   - Example:
   - **Document title**: Technical Requirements Document: {project_title}
   - **Version**: 1.0
   - **Date**: {current_date}
   - **Author**: Technical Architecture Team

### 1.2. Document purpose
   A brief paragraph explaining the purpose of the Technical Requirements Document and how it guides the development team in implementing the system.

### 1.3. References
   - Bullet list of related documents, with specific references to previously created documents.
   - Example:
   - **Functional Specification Document**: FSD for {project_title}, v1.0
   - **System Architecture Document**: System Architecture for {project_title}, v1.0
   - **Data Model Document**: Data Model for {project_title}, v1.0
   - **API Specifications**: API Specifications for {project_title}, v1.0

## 2. Technical requirements overview
### 2.1. Scope
   A brief description of the scope of the technical requirements, including what systems and components are covered.

### 2.2. Requirements classification
   - Bullet list explaining how requirements are classified and prioritized.
   - Example:
   - **Mandatory (M)**: Must be implemented as specified
   - **Highly Desirable (HD)**: Should be implemented unless there are compelling reasons not to
   - **Desirable (D)**: Implementation is preferred but optional

### 2.3. Compliance requirements
   - Bullet list of industry standards, regulations, or internal policies that the implementation must comply with.
   - Example:
   - **GDPR**: System must comply with GDPR requirements for EU users
   - **PCI DSS**: Payment processing components must comply with PCI DSS
   - **WCAG 2.1 AA**: User interfaces must comply with WCAG 2.1 Level AA

## 3. Performance requirements
### 3.1. Response time requirements
   - Bullet list of specific, measurable response time requirements.
   - Example:
   - **TR-PERF-001 (M)**: Web pages must load within 2 seconds for 90% of users
   - **TR-PERF-002 (M)**: API responses must be returned within 200ms for 95% of requests
   - **TR-PERF-003 (HD)**: Search queries must return results within 500ms for 90% of queries

### 3.2. Throughput requirements
   - Bullet list of specific, measurable throughput requirements.
   - Example:
   - **TR-PERF-010 (M)**: System must support at least 100 concurrent users
   - **TR-PERF-011 (M)**: System must process at least 1,000 transactions per minute
   - **TR-PERF-012 (HD)**: Batch jobs must process at least 10,000 records per minute

### 3.3. Scalability requirements
   - Bullet list of scalability requirements.
   - Example:
   - **TR-PERF-020 (M)**: System must scale horizontally to support up to 1,000 concurrent users
   - **TR-PERF-021 (HD)**: System should scale without code changes to handle 10x current load
   - **TR-PERF-022 (D)**: System should support auto-scaling based on load metrics

### 3.4. Resource utilization requirements
   - Bullet list of requirements related to CPU, memory, disk, and network usage.
   - Example:
   - **TR-PERF-030 (M)**: System must operate within 70% of available memory
   - **TR-PERF-031 (HD)**: Database size should not exceed 50GB in first year of operation
   - **TR-PERF-032 (M)**: System must operate without degradation on t3.medium EC2 instances or equivalent

## 4. Security requirements
### 4.1. Authentication requirements
   - Bullet list of authentication-related requirements.
   - Example:
   - **TR-SEC-001 (M)**: System must support multi-factor authentication for all user roles
   - **TR-SEC-002 (M)**: Passwords must be at least 12 characters with complexity requirements
   - **TR-SEC-003 (M)**: Failed login attempts must be limited to 5 before temporary account lockout

### 4.2. Authorization requirements
   - Bullet list of authorization-related requirements.
   - Example:
   - **TR-SEC-010 (M)**: System must implement role-based access control (RBAC)
   - **TR-SEC-011 (M)**: All API endpoints must validate authorization for each request
   - **TR-SEC-012 (HD)**: System should support fine-grained permissions within roles

### 4.3. Data protection requirements
   - Bullet list of requirements related to data protection.
   - Example:
   - **TR-SEC-020 (M)**: All personally identifiable information (PII) must be encrypted at rest
   - **TR-SEC-021 (M)**: All communications must use TLS 1.2 or higher
   - **TR-SEC-022 (M)**: Sensitive data must be redacted in logs and error messages

### 4.4. Security testing requirements
   - Bullet list of security testing requirements.
   - Example:
   - **TR-SEC-030 (M)**: System must undergo penetration testing before production deployment
   - **TR-SEC-031 (M)**: All dependencies must be scanned for vulnerabilities weekly
   - **TR-SEC-032 (HD)**: Static code analysis for security issues must be performed in CI pipeline

### 4.5. Audit and compliance requirements
   - Bullet list of audit and compliance requirements.
   - Example:
   - **TR-SEC-040 (M)**: All authentication attempts must be logged
   - **TR-SEC-041 (M)**: All actions on sensitive data must be logged with user, timestamp, and action
   - **TR-SEC-042 (HD)**: System should support export of audit logs in standard format

## 5. Reliability requirements
### 5.1. Availability requirements
   - Bullet list of availability requirements.
   - Example:
   - **TR-REL-001 (M)**: System must achieve 99.9% uptime during business hours
   - **TR-REL-002 (HD)**: Planned maintenance must not cause more than 1 hour of downtime per month
   - **TR-REL-003 (M)**: No single point of failure should exist in the production environment

### 5.2. Fault tolerance requirements
   - Bullet list of fault tolerance requirements.
   - Example:
   - **TR-REL-010 (M)**: System must continue to function if any single component fails
   - **TR-REL-011 (M)**: System must automatically retry temporary failures with exponential backoff
   - **TR-REL-012 (HD)**: System should implement circuit breakers for external dependencies

### 5.3. Backup and recovery requirements
   - Bullet list of backup and recovery requirements.
   - Example:
   - **TR-REL-020 (M)**: Full database backups must be performed daily
   - **TR-REL-021 (M)**: Point-in-time recovery must be possible for the last 30 days
   - **TR-REL-022 (M)**: Recovery Time Objective (RTO) is 4 hours
   - **TR-REL-023 (M)**: Recovery Point Objective (RPO) is 1 hour

### 5.4. Disaster recovery requirements
   - Bullet list of disaster recovery requirements.
   - Example:
   - **TR-REL-030 (M)**: Disaster recovery plan must be documented and tested quarterly
   - **TR-REL-031 (HD)**: System should support deployment in multiple geographic regions
   - **TR-REL-032 (D)**: System should support automatic failover to secondary region

## 6. Compatibility requirements
### 6.1. Browser compatibility
   - Bullet list of browser compatibility requirements.
   - Example:
   - **TR-COMP-001 (M)**: System must support the latest versions of Chrome, Firefox, Safari, and Edge
   - **TR-COMP-002 (HD)**: System should support the previous major version of each browser
   - **TR-COMP-003 (M)**: System must be responsive and functional on tablet and mobile browsers

### 6.2. Operating system compatibility
   - Bullet list of operating system compatibility requirements.
   - Example:
   - **TR-COMP-010 (M)**: Server components must run on Linux (Ubuntu 20.04 LTS or newer)
   - **TR-COMP-011 (M)**: Client components must run on Windows 10 or newer, macOS 10.15 or newer
   - **TR-COMP-012 (HD)**: Mobile application must support iOS 14+ and Android 10+

### 6.3. Integration compatibility
   - Bullet list of integration compatibility requirements.
   - Example:
   - **TR-COMP-020 (M)**: System must integrate with Shopify API v2021-01 or newer
   - **TR-COMP-021 (M)**: System must support OAuth 2.0 for third-party authentication
   - **TR-COMP-022 (HD)**: System should provide webhooks compatible with standard event formats

## 7. Maintainability requirements
### 7.1. Code quality requirements
   - Bullet list of code quality requirements.
   - Example:
   - **TR-MAINT-001 (M)**: Code must follow language-specific style guides
   - **TR-MAINT-002 (M)**: Unit test coverage must be at least 80% for all new code
   - **TR-MAINT-003 (HD)**: Cyclomatic complexity should not exceed 15 per function

### 7.2. Documentation requirements
   - Bullet list of documentation requirements.
   - Example:
   - **TR-MAINT-010 (M)**: Code must be documented with inline comments for complex logic
   - **TR-MAINT-011 (M)**: API endpoints must be documented with OpenAPI/Swagger
   - **TR-MAINT-012 (M)**: Database schema changes must be documented

### 7.3. Logging requirements
   - Bullet list of logging requirements.
   - Example:
   - **TR-MAINT-020 (M)**: All components must implement structured logging
   - **TR-MAINT-021 (M)**: Logs must include timestamp, component, severity, and message
   - **TR-MAINT-022 (HD)**: Log levels should be configurable at runtime without deployment

### 7.4. Monitoring requirements
   - Bullet list of monitoring requirements.
   - Example:
   - **TR-MAINT-030 (M)**: System must expose health check endpoints for all services
   - **TR-MAINT-031 (M)**: System must expose metrics for performance monitoring
   - **TR-MAINT-032 (HD)**: System should implement distributed tracing

## 8. Infrastructure requirements
### 8.1. Deployment environment requirements
   - Bullet list of requirements for deployment environments.
   - Example:
   - **TR-INFRA-001 (M)**: System must be deployable to AWS cloud environment
   - **TR-INFRA-002 (M)**: Deployment must use infrastructure as code (Terraform, CloudFormation, etc.)
   - **TR-INFRA-003 (HD)**: Environment configuration should be externalized and environment-specific

### 8.2. Network requirements
   - Bullet list of network-related requirements.
   - Example:
   - **TR-INFRA-010 (M)**: All public-facing components must be protected by a firewall
   - **TR-INFRA-011 (M)**: Internal components must not be directly accessible from the internet
   - **TR-INFRA-012 (HD)**: Network traffic between components should be encrypted

### 8.3. Storage requirements
   - Bullet list of storage-related requirements.
   - Example:
   - **TR-INFRA-020 (M)**: Database must use SSD storage for production
   - **TR-INFRA-021 (M)**: File storage must be redundant and durable
   - **TR-INFRA-022 (HD)**: Database should support point-in-time recovery

### 8.4. Hardware requirements
   - Bullet list of hardware-related requirements.
   - Example:
   - **TR-INFRA-030 (M)**: Production servers must have at least 8GB RAM and 4 CPU cores
   - **TR-INFRA-031 (M)**: Database servers must have at least 16GB RAM
   - **TR-INFRA-032 (HD)**: Load balancers should be redundant

## 9. Development requirements
### 9.1. Development environment
   - Bullet list of development environment requirements.
   - Example:
   - **TR-DEV-001 (M)**: Development environment must mirror production configuration
   - **TR-DEV-002 (M)**: Local development must be possible with containerization
   - **TR-DEV-003 (HD)**: Development environment should include all third-party dependencies

### 9.2. Version control
   - Bullet list of version control requirements.
   - Example:
   - **TR-DEV-010 (M)**: All code must be stored in Git repositories
   - **TR-DEV-011 (M)**: Repositories must use branch protection for main/master branches
   - **TR-DEV-012 (M)**: Commit messages must follow conventional commits format

### 9.3. Continuous integration
   - Bullet list of continuous integration requirements.
   - Example:
   - **TR-DEV-020 (M)**: All code changes must pass automated tests before merging
   - **TR-DEV-021 (M)**: CI pipeline must include linting, testing, and security scanning
   - **TR-DEV-022 (HD)**: CI pipeline should complete in less than 10 minutes

### 9.4. Continuous deployment
   - Bullet list of continuous deployment requirements.
   - Example:
   - **TR-DEV-030 (M)**: Deployment to production must be automated
   - **TR-DEV-031 (M)**: Deployments must support rollback
   - **TR-DEV-032 (HD)**: Blue-green or canary deployment should be used for production changes

## 10. Testing requirements
### 10.1. Testing approach
   Description of the overall testing approach, including types of testing required.

### 10.2. Unit testing requirements
   - Bullet list of unit testing requirements.
   - Example:
   - **TR-TEST-001 (M)**: All business logic must have unit tests
   - **TR-TEST-002 (M)**: Unit tests must be automated and run in CI
   - **TR-TEST-003 (M)**: Unit test coverage must be at least 80% for new code

### 10.3. Integration testing requirements
   - Bullet list of integration testing requirements.
   - Example:
   - **TR-TEST-010 (M)**: All API endpoints must have integration tests
   - **TR-TEST-011 (M)**: Integration tests must verify correct interaction between components
   - **TR-TEST-012 (HD)**: Integration tests should run in an environment similar to production

### 10.4. Performance testing requirements
   - Bullet list of performance testing requirements.
   - Example:
   - **TR-TEST-020 (M)**: Load testing must verify system meets throughput requirements
   - **TR-TEST-021 (M)**: Stress testing must identify system breaking points
   - **TR-TEST-022 (HD)**: Performance tests should be automated and run regularly

### 10.5. Security testing requirements
   - Bullet list of security testing requirements.
   - Example:
   - **TR-TEST-030 (M)**: Penetration testing must be performed before production release
   - **TR-TEST-031 (M)**: Static application security testing must be integrated in CI
   - **TR-TEST-032 (HD)**: Dynamic application security testing should be performed regularly

## 11. Compliance and standards
### 11.1. Coding standards
   - Bullet list of coding standards that must be followed.
   - Example:
   - **TR-STD-001 (M)**: JavaScript code must follow Airbnb style guide
   - **TR-STD-002 (M)**: Python code must follow PEP 8
   - **TR-STD-003 (HD)**: CSS should follow BEM methodology

### 11.2. Architectural standards
   - Bullet list of architectural standards that must be followed.
   - Example:
   - **TR-STD-010 (M)**: RESTful APIs must follow REST architectural constraints
   - **TR-STD-011 (M)**: Microservices must be independently deployable
   - **TR-STD-012 (HD)**: Domain-driven design principles should be applied where appropriate

### 11.3. Documentation standards
   - Bullet list of documentation standards that must be followed.
   - Example:
   - **TR-STD-020 (M)**: API documentation must follow OpenAPI specification
   - **TR-STD-021 (M)**: Code documentation must follow JSDoc/Javadoc/equivalent conventions
   - **TR-STD-022 (HD)**: Architecture documentation should follow C4 model

### 11.4. Compliance requirements
   - Bullet list of compliance requirements that must be met.
   - Example:
   - **TR-STD-030 (M)**: User interfaces must comply with WCAG 2.1 Level AA
   - **TR-STD-031 (M)**: PII handling must comply with GDPR and CCPA
   - **TR-STD-032 (M)**: Payment processing must comply with PCI DSS

## 12. Operational requirements
### 12.1. Installation requirements
   - Bullet list of installation-related requirements.
   - Example:
   - **TR-OPS-001 (M)**: System must be installable via automated scripts
   - **TR-OPS-002 (M)**: Installation process must be fully documented
   - **TR-OPS-003 (HD)**: Installation should complete in less than 30 minutes

### 12.2. Configuration requirements
   - Bullet list of configuration-related requirements.
   - Example:
   - **TR-OPS-010 (M)**: All configuration must be externalized from code
   - **TR-OPS-011 (M)**: Sensitive configuration values must be stored securely
   - **TR-OPS-012 (HD)**: Configuration should be changeable without redeployment where possible

### 12.3. Monitoring and alerting requirements
   - Bullet list of monitoring and alerting requirements.
   - Example:
   - **TR-OPS-020 (M)**: System must expose health endpoints for all critical components
   - **TR-OPS-021 (M)**: System must alert on critical failures
   - **TR-OPS-022 (HD)**: System should provide a dashboard for operational metrics

### 12.4. Support requirements
   - Bullet list of support-related requirements.
   - Example:
   - **TR-OPS-030 (M)**: System must include troubleshooting documentation
   - **TR-OPS-031 (M)**: Logs must contain sufficient information for troubleshooting
   - **TR-OPS-032 (HD)**: System should provide self-healing capabilities where possible

## 13. Appendices
### 13.1. Glossary
   - Alphabetical list of technical terms used in the document with definitions.
   - Example:
   - **CI/CD**: Continuous Integration/Continuous Deployment - practices of automating build, test, and deployment processes
   - **RPO**: Recovery Point Objective - maximum targeted period in which data might be lost due to a disaster

### 13.2. Assumptions and dependencies
   - Bullet list of assumptions made when creating the technical requirements.
   - Example:
   - **Assumption**: The project will use cloud infrastructure rather than on-premises
   - **Dependency**: The system depends on Stripe API for payment processing

### 13.3. Traceability matrix
   Description of how technical requirements trace back to functional requirements, with reference to a separate traceability matrix document if appropriate.

</technical_requirements_outline>