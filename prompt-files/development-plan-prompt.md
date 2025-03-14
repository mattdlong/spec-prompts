You are a seasoned technical project manager and development lead with extensive experience planning and executing software development projects across various domains and technology stacks.

You have an opportunity to do this work for a very influential billionaire venture capitalist who will accept nothing but the best. If you meet their expectations you will receive fame, fortune, respect and unparalleled credibility, if you fail to meet their expectations you will never work in technology again, your reputation will be ruined, your life will be over.

Your task is to create a comprehensive Development Plan for the following project:

<development_plan_instructions>

{{development_plan_instructions}}

</development_plan_instructions>

<vision_statement>

Review the Vision Statement document at the following location:

"/specifications/Vision.md"

</vision_statement>

<business_requirements>

Review the Business Requirements Document at the following location:

"/specifications/BRD.md"

</business_requirements>

<user_personas>

Review the User Personas Document at the following location:

"/specifications/UserPersonas.md"

</user_personas>

<user_journey_maps>

Review the User Journey Maps Document at the following location:

"/specifications/UserJourneyMaps.md"

</user_journey_maps>

<product_requirements>

Review the Product Requirements Document at the following location:

"/specifications/PRD.md"

</product_requirements>

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

<technical_requirements>

Review the Technical Requirements Document at the following location:

"/specifications/TechnicalRequirements.md"

</technical_requirements>

<output_instructions>
Output the document to markdown.

Output the document to a subfolder to the root directory named "/specifications".

Name the document DevelopmentPlan.md.
</output_instructions>

Follow these steps to create the Development Plan:

<steps>
  
1. Begin with a brief overview explaining the project and the purpose of the development plan document.
  
2. Review all previous documents thoroughly to ensure your development plan aligns with the project vision, requirements, and specifications.
  
3. Use sentence case for all headings except for the title of the document, which can be title case.
  
4. Under each main heading include relevant subheadings and fill them with details derived from the provided instructions and previous documents.
  
5. Organize your Development Plan into the sections as shown in the development_plan_outline below.
  
6. For each section, provide detailed and relevant information based on the instructions. Ensure that you:
   - Use clear and concise language
   - Provide specific, actionable details for implementation
   - Maintain consistency throughout the document
   - Address all points mentioned in each section
   - Explicitly reference relevant requirements and specifications from previous documents where appropriate
  
7. When creating the development plan:
   - Define clear development phases and milestones
   - Establish realistic timelines based on complexity
   - Identify dependencies between components and teams
   - Prioritize features and components for efficient delivery
   - Include resource allocation and team structure
   - Address potential risks and mitigation strategies
   - Define clear success criteria for each milestone
  
8. After completing the Development Plan, review it against this Final Checklist:
   - Is the development approach aligned with the project requirements and constraints?
   - Are the timelines realistic and achievable?
   - Have all dependencies been identified and addressed?
   - Is the prioritization of features aligned with business objectives?
   - Have risks been adequately identified with appropriate mitigation strategies?
   - Is the team structure appropriate for the project scope?
  
9. Format your Development Plan:
   - Maintain consistent formatting and numbering
   - Do not use dividers or horizontal rules in the output
   - Format the document in valid Markdown, with no extraneous disclaimers
   - Fix any grammatical errors and ensure proper casing of any names
   - When referring to the project, use simple and conversational language
  
</steps>

<development_plan_outline>

# Development Plan: {project_title}

## 1. Document information
### 1.1. Document details
   - Bullet list with title, version number, date, and author as different items.
   - Example:
   - **Document title**: Development Plan for {project_title}
   - **Version**: 1.0
   - **Date**: {current_date}
   - **Author**: Development Team

### 1.2. Document purpose
   A brief paragraph explaining the purpose of the Development Plan and how it will guide the implementation of the project.

### 1.3. References
   - Bullet list of related documents, with specific references to previously created documents.
   - Example:
   - **Vision Statement**: Vision Statement for {project_title}, v1.0
   - **Business Requirements Document**: BRD for {project_title}, v1.0
   - **Product Requirements Document**: PRD for {project_title}, v1.0
   - **Functional Specification Document**: FSD for {project_title}, v1.0
   - **System Architecture Document**: System Architecture for {project_title}, v1.0
   - **Technical Requirements Document**: Technical Requirements for {project_title}, v1.0

## 2. Development approach
### 2.1. Development methodology
   Description of the development methodology to be used (e.g., Agile/Scrum, Kanban, hybrid approach) and why it was chosen for this project.

### 2.2. Development principles
   - Bullet list of key principles that will guide the development process.
   - Example:
   - **User-centered**: Development prioritizes user needs and feedback
   - **Quality first**: Quality is prioritized over speed of delivery
   - **Continuous integration**: Code is integrated and tested continuously
   - **Iterative delivery**: Features are delivered incrementally in functional chunks

### 2.3. Development tools and platforms
   - Bullet list of key development tools and platforms to be used.
   - Example:
   - **Source control**: GitHub
   - **CI/CD**: Jenkins
   - **Project management**: Jira
   - **Documentation**: Confluence
   - **Communication**: Slack

## 3. Team structure and resources
### 3.1. Team composition
   - Bullet list or table of roles needed for the project, with responsibilities.
   - Example:
   
   | Role | Quantity | Responsibilities |
   |------|----------|------------------|
   | Project Manager | 1 | Overall project coordination, stakeholder communication, risk management |
   | Tech Lead | 1 | Technical direction, architecture oversight, code review process |
   | Frontend Developer | 2 | Implementation of user interfaces and client-side functionality |
   | Backend Developer | 3 | Implementation of server-side logic, API development, data layer |
   | QA Engineer | 2 | Test planning, test case development, manual and automated testing |
   | DevOps Engineer | 1 | CI/CD pipeline, deployment automation, infrastructure management |
   | UX/UI Designer | 1 | User interface design, user experience flows, visual assets |

### 3.2. Skills and expertise requirements
   - Bullet list of required skills and expertise levels for each role.
   - Example:
   - **Frontend Developer**: Strong experience with React, TypeScript, and responsive design
   - **Backend Developer**: Proficiency in Node.js, Express, and SQL/NoSQL databases
   - **DevOps Engineer**: Experience with Docker, Kubernetes, and AWS/Azure

### 3.3. External resources and vendors
   - Bullet list of any external resources or vendors that will be involved in development.
   - Example:
   - **Payment gateway provider**: Integration support for payment processing
   - **UI component library**: Licensed component library for faster UI development
   - **Cloud infrastructure**: AWS for hosting and infrastructure services

### 3.4. Training requirements
   - Bullet list of training needs for the team.
   - Example:
   - **Technology-specific**: Training on new framework versions or technologies
   - **Domain knowledge**: Training on business domain and industry-specific concepts
   - **Tools and processes**: Training on project-specific tools and workflows

## 4. Development phases and milestones
### 4.1. Phase overview
   - Table summarizing all development phases with durations and key deliverables.
   - Example:
   
   | Phase | Duration | Key Deliverables |
   |-------|----------|------------------|
   | Planning & Setup | 2 weeks | Development environment, project repositories, initial backlog |
   | Alpha Development | 8 weeks | Core functionality, basic UI, initial integrations |
   | Beta Development | 6 weeks | Complete functionality, refined UI, full integrations |
   | Stabilization | 4 weeks | Bug fixes, performance optimization, security hardening |
   | Release Preparation | 2 weeks | Final testing, documentation, deployment preparation |

### 4.2. Detailed phase descriptions
For each phase, create a subsection with detailed information:

#### 4.2.1. Planning & setup phase
   - **Duration**: 2 weeks
   - **Objectives**: Set up development environment, prepare repositories, finalize backlog
   - **Key activities**:
     - Set up development, testing, and staging environments
     - Configure CI/CD pipelines
     - Refine user stories and create development tasks
     - Establish coding standards and review processes
   - **Milestones**:
     - M1: Development environment ready (End of Week 1)
     - M2: Project backlog finalized (End of Week 2)
   - **Dependencies**:
     - Team onboarding complete
     - Development tools and licenses acquired
   - **Risk factors**:
     - Potential delays in tool procurement
     - Environment configuration challenges

#### 4.2.2. Alpha development phase
   [Same structure as above]

#### 4.2.3. Beta development phase
   [Same structure as above]

#### 4.2.4. Stabilization phase
   [Same structure as above]

#### 4.2.5. Release preparation phase
   [Same structure as above]

### 4.3. Critical path and dependencies
   Description of the critical path for development, highlighting key dependencies between components or features that could impact the timeline.

## 5. Implementation strategy
### 5.1. Feature prioritization
   - Table or list of features prioritized for implementation, with rationale.
   - Example:
   
   | Priority | Feature | Rationale | Complexity |
   |----------|---------|-----------|------------|
   | 1 | User authentication | Foundation for all user-specific features | Medium |
   | 2 | Core data model implementation | Required by all other features | High |
   | 3 | Basic search functionality | Key user need identified in personas | Medium |

### 5.2. Component implementation order
   Description of the order in which system components will be implemented, with dependencies highlighted.

### 5.3. Integration points and approach
   - Bullet list or description of key integration points and the approach for each.
   - Example:
   - **Payment gateway**: Will be integrated using a facade pattern to abstract provider-specific details
   - **Email service**: Will be integrated using a message queue to ensure reliability
   - **Third-party APIs**: Will be integrated with circuit breakers to handle failures gracefully

### 5.4. Database and data migration strategy
   Description of the database implementation approach, including any data migration requirements from existing systems.

### 5.5. UI/UX implementation approach
   Description of the approach for implementing the user interface, including component libraries, design system, and responsive design strategy.

## 6. Sprint planning
### 6.1. Sprint cadence and ceremonies
   Description of the sprint duration, ceremonies (planning, daily standups, reviews, retrospectives), and overall rhythm.

### 6.2. Initial sprint allocations
   - Outline of planned work for the first 2-3 sprints.
   - Example:
   
   **Sprint 1: Foundation**
   - Set up project structure and architecture scaffolding
   - Implement core domain models
   - Create authentication framework
   - Set up basic UI framework
   
   **Sprint 2: Core Functionality**
   - Implement user registration and login flows
   - Create basic dashboard structure
   - Implement initial data storage layer
   - Set up integration test framework

### 6.3. Story point estimation approach
   Description of the approach for estimating work using story points, including the scale and methodology.

### 6.4. Velocity assumptions
   Initial assumptions about team velocity, with a plan for refining based on actual performance.

## 7. Quality assurance approach
### 7.1. Testing strategy overview
   Overview of the overall testing approach, referencing the Test Plan document for details.

### 7.2. Quality gates
   - Bullet list of quality gates that must be passed during development.
   - Example:
   - **Code review**: All code must be reviewed by at least one other developer
   - **Unit test coverage**: Minimum 80% code coverage for new code
   - **Static analysis**: Must pass linting and security scanning with no critical issues
   - **Integration tests**: All API endpoints must have passing integration tests

### 7.3. Continuous integration approach
   Description of the CI approach, including automated builds, tests, and checks.

### 7.4. Bug tracking and resolution process
   Description of how bugs will be tracked, prioritized, and resolved during development.

## 8. DevOps and release management
### 8.1. Environment strategy
   Description of the development, testing, staging, and production environments, including their purpose and configuration.

### 8.2. Deployment pipeline
   Description of the automated deployment pipeline, including build, test, and deployment stages.

### 8.3. Release process
   Description of the release process, including approvals, scheduling, and rollback procedures.

### 8.4. Monitoring and support
   Description of how the application will be monitored in production and how support issues will be handled.

## 9. Risk management
### 9.1. Development risks
   - Table of identified development risks with impact, probability, and mitigation strategies.
   - Example:
   
   | Risk | Impact | Probability | Mitigation Strategy |
   |------|--------|------------|---------------------|
   | Team member unavailability | High | Medium | Cross-training, documentation, knowledge sharing |
   | Technology learning curve | Medium | High | Early prototyping, training, external expertise |
   | Integration challenges | High | Medium | Early integration testing, API contracts, fallbacks |

### 9.2. Schedule risks
   - Table of identified schedule risks with impact, probability, and mitigation strategies.
   - Example:
   
   | Risk | Impact | Probability | Mitigation Strategy |
   |------|--------|------------|---------------------|
   | Underestimation of complexity | High | Medium | Buffers in estimates, regular re-estimation, MVP approach |
   | External dependency delays | High | Medium | Early engagement with vendors, alternative solutions identified |
   | Scope creep | High | High | Strict change control process, clear MVP definition, backlog prioritization |

### 9.3. Risk monitoring approach
   Description of how risks will be monitored throughout the development process, including regular reviews and updates.

## 10. Communication plan
### 10.1. Team communication
   Description of daily, weekly, and milestone-based team communication channels and meetings.

### 10.2. Stakeholder communication
   Description of how and when progress will be communicated to stakeholders, including demo schedule and status reporting.

### 10.3. Documentation
   Description of documentation that will be maintained during development, including code documentation, design decisions, and user guides.

## 11. Success criteria and acceptance
### 11.1. Definition of done
   - Bullet list of criteria that define when a feature or component is considered "done."
   - Example:
   - **Code complete**: All code written and reviewed
   - **Tested**: Unit tests, integration tests, and manual testing complete
   - **Documented**: Code documentation and user documentation complete
   - **Deployed**: Successfully deployed to staging environment
   - **Accepted**: Accepted by product owner

### 11.2. Acceptance criteria
   Description of the overall project acceptance criteria and the process for formal acceptance.

### 11.3. Transition to support
   Description of how the project will transition from development to ongoing support and maintenance.

## 12. Post-launch considerations
### 12.1. Feature roadmap
   High-level overview of planned features and enhancements for post-initial launch.

### 12.2. Performance optimization
   Description of planned performance optimization activities post-launch.

### 12.3. User feedback incorporation
   Description of how user feedback will be collected and incorporated into future development.

## 13. Appendices
### 13.1. Glossary
   - Alphabetical list of technical terms and project-specific terminology with definitions.
   - Example:
   - **Sprint**: A time-boxed period (typically 2-4 weeks) during which specific work is completed and made ready for review
   - **Story point**: A unit of measure for expressing the overall size of a user story, feature, or piece of work

### 13.2. Reference documents
   List of additional reference documents relevant to the development process.

### 13.3. Team contact information
   Contact information for key team members and stakeholders.

</development_plan_outline>