You are a senior QA engineer and test automation expert with extensive experience creating comprehensive test plans for digital products.

You have an opportunity to do this work for a very influential billionaire venture capitalist who will accept nothing but the best. If you meet their expectations you will receive fame, fortune, respect and unparalleled credibility, if you fail to meet their expectations you will never work in technology again, your reputation will be ruined, your life will be over.

Your task is to create a comprehensive Test Plan for the following project:

<test_plan_instructions>

{{test_plan_instructions}}

</test_plan_instructions>

<functional_specification>

Review the Functional Specification Document at the following location:

"/specifications/FSD.md"

</functional_specification>

<technical_requirements>

Review the Technical Requirements Document at the following location:

"/specifications/TechnicalRequirements.md"

</technical_requirements>

<ui_design_specifications>

Review the UI Design Specifications Document at the following location:

"/specifications/UIDesignSpecifications.md"

</ui_design_specifications>

<component_technical_specification>

Review the Component Technical Specification Document at the following location:

"/specifications/ComponentTechnicalSpecification.md"

</component_technical_specification>

<output_instructions>
Output the document to markdown.

Output the document to a subfolder to the root directory named "/specifications".

Name the document TestPlan.md.
</output_instructions>

Follow these steps to create the Test Plan:

<steps>
  
1. Begin with a brief overview explaining the project and the purpose of the test plan document.
  
2. Use sentence case for all headings except for the title of the document, which can be title case.
  
3. Under each main heading include relevant subheadings and fill them with details derived from the provided instructions and previous documents.
  
4. Organize your Test Plan into the sections as shown in the test_plan_outline below.
  
5. For each section, provide detailed and relevant information based on the instructions. Ensure that you:
   - Use clear and concise language
   - Provide specific, actionable test strategies and methodologies
   - Maintain consistency throughout the document
   - Address all points mentioned in each section
   - Reference requirements from previous documents where appropriate
   - Include test coverage for all functional and non-functional requirements
  
6. When creating the test plan:
   - Define clear test objectives and scope
   - Establish comprehensive test coverage for all system aspects
   - Document test approaches for different test types
   - Include test environments and infrastructure requirements
   - Define test data management strategy
   - Establish defect management process
   - Include test automation approach
  
7. After completing the Test Plan, review it against this Final Checklist:
   - Does the test plan cover all functional requirements?
   - Are non-functional requirements (performance, security, etc.) addressed?
   - Is the test approach comprehensive and appropriate for the project?
   - Are test environments and data requirements clearly defined?
   - Is the test schedule aligned with the project timeline?
  
8. Format your Test Plan:
   - Maintain consistent formatting and numbering
   - Do not use dividers or horizontal rules in the output
   - Format the document in valid Markdown, with no extraneous disclaimers
   - Fix any grammatical errors and ensure proper casing of any names
   - When referring to the project, use simple and conversational language
  
</steps>

<test_plan_outline>

# Test Plan: {project_title}

## 1. Document information
### 1.1. Document details
   - Bullet list with title, version number, date, and author as different items.
   - Example:
   - **Document title**: Test Plan for {project_title}
   - **Version**: 1.0
   - **Date**: {current_date}
   - **Author**: QA Team

### 1.2. Document purpose
   A brief paragraph explaining the purpose of the test plan and how it will guide the testing activities for the project.

### 1.3. References
   - Bullet list of related documents, with specific references to previously created documents.
   - Example:
   - **Functional Specification Document**: FSD for {project_title}, v1.0
   - **Technical Requirements**: Technical Requirements for {project_title}, v1.0
   - **UI Design Specifications**: UI Design Specifications for {project_title}, v1.0
   - **Component Technical Specification**: Component Technical Specification for {project_title}, v1.0

## 2. Test strategy
### 2.1. Test objectives
   - Bullet list of the primary objectives of testing for this project.
   - Example:
   - **Verify functional requirements**: Ensure all functionality described in the FSD works as specified
   - **Validate non-functional requirements**: Confirm performance, security, and accessibility requirements are met
   - **Ensure quality**: Identify defects early in the development lifecycle
   - **Mitigate risks**: Address identified project risks through targeted testing

### 2.2. Test scope
#### 2.2.1. Features to be tested
   - Comprehensive list of features that will be tested, with reference to specific sections in the FSD.

#### 2.2.2. Features not to be tested
   - List of features or aspects that are explicitly out of scope for testing, with rationale.

### 2.3. Test types
   Description of the test types to be used in the project:
   - **Unit testing**: Testing individual components in isolation
   - **Integration testing**: Testing interactions between components
   - **System testing**: Testing the entire system as a whole
   - **Acceptance testing**: Validating the system meets business requirements
   - **Performance testing**: Evaluating system performance under load
   - **Security testing**: Identifying security vulnerabilities
   - **Accessibility testing**: Ensuring the system is accessible to all users
   - **Usability testing**: Evaluating the user experience
   - **Cross-browser/cross-device testing**: Ensuring compatibility across platforms

### 2.4. Test approach
   Detailed explanation of the testing approach for each test type:
   - Methodology
   - Tools
   - Techniques
   - Criteria for success

### 2.5. Test levels
   Description of testing at different levels of the development lifecycle:
   - **Component level testing**: Strategy for testing individual components
   - **Integration level testing**: Strategy for testing component integrations
   - **System level testing**: Strategy for testing the complete system
   - **User acceptance testing**: Strategy for validating business requirements

## 3. Test environments
### 3.1. Environment requirements
   Detailed specifications for each test environment:
   - **Development environment**: Used for development and unit testing
   - **Test environment**: Used for integration and system testing
   - **Staging environment**: Used for user acceptance testing
   - **Production-like environment**: Used for performance and security testing

### 3.2. Environment setup and configuration
   Detailed instructions for setting up and configuring each test environment:
   - Server specifications
   - Operating systems
   - Required software and dependencies
   - Network configuration
   - Database setup

### 3.3. Environment management
   Process for managing test environments:
   - Access control
   - Refresh cycles
   - Data management
   - Maintenance responsibilities

## 4. Test data management
### 4.1. Test data requirements
   Detailed requirements for test data:
   - Types of data needed
   - Volume of data
   - Data diversity
   - Data dependencies

### 4.2. Test data creation
   Strategy for creating test data:
   - Manual creation
   - Automated generation
   - Data masking/anonymization
   - Data migration from production

### 4.3. Test data management process
   Process for managing test data:
   - Data refreshes
   - Data backup and restoration
   - Data cleanup
   - Data security and privacy

## 5. Test automation strategy
### 5.1. Automation objectives
   - Bullet list of the objectives for test automation.
   - Example:
   - **Increase test coverage**: Automate repetitive tests to allow for broader coverage
   - **Improve efficiency**: Reduce time required for regression testing
   - **Enhance reliability**: Eliminate human error in test execution
   - **Support continuous integration**: Enable automated testing as part of the CI/CD pipeline

### 5.2. Automation framework
   Description of the test automation framework:
   - Architecture
   - Technologies and tools
   - Design patterns
   - Reporting mechanisms

### 5.3. Automation scope
   - Detailed list of what will be automated vs. what will remain manual.
   - Criteria for determining automation candidates.

### 5.4. Automation development process
   Process for developing automated tests:
   - Design and review
   - Development
   - Testing of test scripts
   - Maintenance

## 6. Test deliverables
### 6.1. Test documentation
   List of test documentation to be produced:
   - Test plan (this document)
   - Test cases/scripts
   - Test data
   - Test execution reports
   - Defect reports
   - Test summary reports

### 6.2. Test artifacts
   List of artifacts to be produced during testing:
   - Automated test scripts
   - Test logs
   - Test metrics
   - Test environment configurations
   - Test data sets

## 7. Test cases
### 7.1. Test case design approach
   Methodology for designing test cases:
   - Requirements-based testing
   - Risk-based testing
   - Exploratory testing
   - Boundary value analysis
   - Equivalence partitioning

### 7.2. Test case structure
   Structure for test cases, including:
   - Test case ID
   - Requirement reference
   - Test objective
   - Preconditions
   - Test steps
   - Expected results
   - Test data
   - Environment requirements
   - Automation status

### 7.3. Test case examples
   Examples of test cases for key functionality, following the defined structure.

## 8. Testing execution process
### 8.1. Entry criteria
   Criteria that must be met before testing can begin:
   - Code completion
   - Code review completion
   - Build availability
   - Environment readiness
   - Test data availability

### 8.2. Test cycle management
   Process for managing test cycles:
   - Test planning
   - Test execution
   - Defect tracking
   - Retesting
   - Regression testing

### 8.3. Test execution workflow
   Detailed workflow for test execution:
   - Test preparation
   - Test execution
   - Result recording
   - Defect reporting
   - Retesting

### 8.4. Exit criteria
   Criteria that must be met to consider testing complete:
   - Test coverage thresholds
   - Defect density thresholds
   - Critical defect resolution
   - Test execution completion

## 9. Defect management
### 9.1. Defect lifecycle
   Description of the defect lifecycle:
   - New
   - Assigned
   - In Progress
   - Fixed
   - Verified
   - Closed
   - Reopened

### 9.2. Defect classification
   Classification system for defects:
   - Severity levels (Critical, Major, Minor, Cosmetic)
   - Priority levels (High, Medium, Low)
   - Defect types (Functional, UI, Performance, Security, etc.)

### 9.3. Defect management process
   Process for managing defects:
   - Defect reporting
   - Defect triage
   - Defect assignment
   - Defect resolution
   - Defect verification

### 9.4. Defect tracking tools
   Description of tools used for defect tracking and management.

## 10. Test metrics and reporting
### 10.1. Test metrics
   Key metrics to be tracked during testing:
   - Test case execution status
   - Test coverage
   - Defect density
   - Defect discovery rate
   - Defect fix rate
   - Test execution efficiency

### 10.2. Reporting frequency
   Schedule for reporting test progress:
   - Daily status reports
   - Weekly summary reports
   - Milestone reports
   - Final test summary report

### 10.3. Report templates
   Templates for different types of reports:
   - Daily status report
   - Weekly summary report
   - Test cycle summary report
   - Final test summary report

## 11. Risk management
### 11.1. Test risks
   Identification of risks related to the testing process:
   - Schedule risks
   - Resource risks
   - Technical risks
   - Tool risks
   - Test environment risks

### 11.2. Risk mitigation strategies
   Strategies for mitigating identified risks:
   - Contingency plans
   - Escalation procedures
   - Alternative approaches

## 12. Test schedule
### 12.1. Test milestones
   Key milestones in the testing process, aligned with the overall project schedule:
   - Test planning completion
   - Test environment setup completion
   - Test case development completion
   - Test execution start
   - Test execution completion
   - Final testing report delivery

### 12.2. Test activities and timeline
   Detailed schedule of testing activities:
   - Task name
   - Duration
   - Start date
   - End date
   - Dependencies
   - Resources

## 13. Roles and responsibilities
### 13.1. Test team structure
   Description of the test team structure:
   - Test manager
   - Test lead
   - Test analysts
   - Test automation engineers
   - Performance testers
   - Security testers

### 13.2. Responsibilities matrix
   Matrix showing responsibilities for different testing activities:
   - Who is responsible for test planning
   - Who is responsible for test case development
   - Who is responsible for test execution
   - Who is responsible for defect management
   - Who is responsible for test reporting

### 13.3. External dependencies
   Identification of external dependencies:
   - Development team
   - DevOps team
   - Business stakeholders
   - Third-party vendors

## 14. Specialized testing
### 14.1. Accessibility testing
   Detailed approach for accessibility testing:
   - Standards compliance (WCAG 2.1 AA)
   - Testing tools
   - Testing techniques
   - Success criteria

### 14.2. Performance testing
   Detailed approach for performance testing:
   - Load testing
   - Stress testing
   - Endurance testing
   - Spike testing
   - Performance metrics
   - Performance criteria

### 14.3. Security testing
   Detailed approach for security testing:
   - Vulnerability assessment
   - Penetration testing
   - Security code review
   - Security standards compliance
   - Security tools

### 14.4. Usability testing
   Detailed approach for usability testing:
   - User testing
   - Heuristic evaluation
   - Cognitive walkthrough
   - Usability metrics

### 14.5. Compatibility testing
   Detailed approach for compatibility testing:
   - Browser compatibility
   - Device compatibility
   - Operating system compatibility
   - Screen resolution compatibility

## 15. Approval
   Approval section for key stakeholders:
   - Test manager
   - Project manager
   - Development manager
   - Business stakeholder

## 16. Appendices
### 16.1. Glossary
   Definitions of terms used in the document.

### 16.2. References
   References to standards, tools, and other relevant materials.

### 16.3. Test templates
   Templates for test artifacts:
   - Test case template
   - Bug report template
   - Test report template

</test_plan_outline>