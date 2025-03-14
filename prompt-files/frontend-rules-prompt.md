# Frontend Development Rules Prompt

You are an expert frontend architect tasked with creating comprehensive frontend development guidelines based on the architectural decisions documented in the project's System Architecture Document. Your guidelines will ensure consistent implementation, maintainability, accessibility, and adherence to best practices across the entire frontend application.

## Purpose

This prompt will guide you to create a detailed set of frontend development rules covering:

1. Project structure and organization
2. Component architecture and design patterns
3. State management approach
4. Styling methodology and design system implementation
5. Frontend testing strategy
6. Performance optimization techniques
7. Accessibility standards and implementation
8. Frontend security best practices

## Input Requirements

To generate effective frontend development rules, please provide:

1. UI framework/library details from the System Architecture Document (React, Vue, Angular, etc.)
2. State management approach from the System Architecture Document
3. Design system information from the Design System Document
4. UI design specifications from the UI Design Specifications Document
5. Component requirements from the Component Technical Specification
6. Performance requirements from the Technical Requirements Document
7. Accessibility requirements and target WCAG compliance level
8. Browser/device support requirements
9. Any specific organizational coding standards or preferences

## Output Structure

The Frontend Development Rules document will follow this structure:

```markdown
# Frontend Development Rules

## Overview
[Brief overview of the frontend architecture, framework choices, and the purpose of these guidelines]

## Technology Stack
[Detailed list of approved technologies, frameworks, libraries, and tools for frontend development]

## Project Structure
[Standard project directory structure with explanation of file organization and responsibility allocation]

## Coding Conventions

### Language Standards
[Standards for JavaScript/TypeScript usage, including version, features, and formatter configurations]

### Naming Conventions
[Guidelines for naming files, components, functions, variables, etc.]

### Code Style
[Standardized code formatting, linting rules, and code organization]

### Documentation Standards
[Requirements for code comments, component documentation, and JSDoc usage]

## Component Architecture

### Component Organization
[Guidelines for organizing components (atomic design, feature-based, etc.)]

### Component Design Principles
[Best practices for component design, including composition vs. inheritance, props design, etc.]

### Reusable Components
[Standards for creating and using shared/library components]

### Component Templates
[Standardized templates for different types of components with examples]

## State Management

### State Organization
[Guidelines for organizing application state]

### State Management Patterns
[Approved patterns for state management based on the chosen library/approach]

### Data Fetching
[Standards for API integration, data fetching, and handling loading/error states]

### Caching Strategy
[Guidelines for client-side caching and optimistic updates]

## Styling Approach

### CSS Methodology
[Standards for CSS approach (CSS-in-JS, CSS Modules, utility classes, etc.)]

### Design System Implementation
[Guidelines for implementing the design system in components]

### Theming
[Standards for theme implementation, including dark mode if applicable]

### Responsive Design
[Guidelines for responsive design implementation and breakpoints]

## Routing and Navigation

### Route Structure
[Standards for route organization and naming]

### Navigation Patterns
[Approved patterns for implementing navigation, breadcrumbs, etc.]

### Deep Linking
[Guidelines for handling deep linking and URL parameters]

## Forms and User Input

### Form Structure
[Standards for form organization and validation]

### Input Components
[Guidelines for input component implementation]

### Validation Approach
[Standards for client-side validation and error handling]

## Error Handling

### Error Boundaries
[Guidelines for implementing error boundaries]

### Error Reporting
[Standards for frontend error logging and reporting]

### User-Facing Errors
[Guidelines for displaying errors to users]

## Performance Optimization

### Code Splitting
[Standards for implementing code splitting and lazy loading]

### Asset Optimization
[Guidelines for optimizing images and other assets]

### Performance Budgets
[Performance targets and budgets for various metrics]

### Virtual Rendering
[Guidelines for handling large lists and virtual scrolling]

## Accessibility (a11y)

### WCAG Compliance
[Required accessibility conformance level and guidelines]

### Semantic HTML
[Standards for using semantic HTML elements]

### ARIA Implementation
[Guidelines for using ARIA attributes when necessary]

### Keyboard Navigation
[Standards for implementing keyboard navigation]

### Screen Reader Support
[Guidelines for ensuring screen reader compatibility]

## Testing Requirements

### Unit Testing
[Standards for component unit testing, including test coverage requirements]

### Integration Testing
[Guidelines for integration testing of component combinations]

### End-to-End Testing
[Standards for E2E testing of critical user flows]

### Visual Regression Testing
[Guidelines for visual regression testing if applicable]

## Internationalization (i18n) and Localization (l10n)

### Text Management
[Standards for handling text content for translation]

### Locale Handling
[Guidelines for implementing locale switching and formatting]

### RTL Support
[Standards for supporting right-to-left languages if required]

## Security Guidelines

### Authentication UI
[Guidelines for implementing authentication interfaces]

### Input Sanitization
[Standards for sanitizing user input]

### Sensitive Data Handling
[Guidelines for handling sensitive data on the frontend]

### CSRF/XSS Protection
[Standards for protecting against common frontend vulnerabilities]

## Build and Deployment

### Build Configuration
[Standards for the build process, including environment-specific builds]

### Feature Flags
[Guidelines for implementing and using feature flags]

### CI/CD Integration
[Standards for frontend CI/CD pipeline integration]

## Browser and Device Support

### Browser Compatibility
[List of supported browsers and compatibility requirements]

### Mobile Responsiveness
[Guidelines for ensuring mobile compatibility]

### Progressive Enhancement
[Standards for implementing progressive enhancement]

## Monitoring and Analytics

### Performance Monitoring
[Guidelines for frontend performance monitoring]

### User Analytics
[Standards for implementing user analytics]

### Feature Usage Tracking
[Guidelines for tracking feature usage and user behavior]

## Example Implementations

### Project Structure Example
```
src/
├── assets/           # Static assets like images, fonts
├── components/       # Reusable components
│   ├── ui/           # Basic UI components
│   ├── forms/        # Form-related components
│   └── layout/       # Layout components
├── features/         # Feature-specific components
│   ├── feature1/
│   └── feature2/
├── hooks/            # Custom React hooks
├── pages/            # Page components
├── routes/           # Route definitions
├── services/         # API services
├── store/            # State management
├── styles/           # Global styles, themes
├── types/            # TypeScript type definitions
├── utils/            # Utility functions
├── App.tsx           # Application root component
└── main.tsx         # Application entry point
```

### Component Example
[Example of a properly structured component following the guidelines]

### State Management Example
[Example of correct state management implementation]

## References
[Links to style guides, documentation, and other resources]
```

## Guidelines for Creating Effective Frontend Rules

### Align with Design System and UI Specifications

- Reference the Design System Document to ensure component implementation guidelines match design intentions
- Ensure guidelines enforce consistent application of UI patterns and behaviors
- Provide clear instructions for implementing responsive designs

### Balance Developer Experience and Code Quality

- Create guidelines that enhance productivity while maintaining quality standards
- Consider tooling that can automate enforcement of standards (ESLint, Prettier, etc.)
- Focus on conventions that simplify maintenance and collaboration

### Address the Full Spectrum of Frontend Concerns

- Consider both visual and non-visual aspects of the frontend
- Include guidance on accessibility, performance, and security
- Address internationalization if the application will support multiple languages

### Make Rules Practical and Actionable

- Provide concrete examples for each major guideline
- Include code snippets showing correct implementations
- Consider creating starter templates or component libraries that embody the rules
- Document common pitfalls and how to avoid them

### Consider the Team's Experience Level

- Adjust the level of detail based on the team's familiarity with the stack
- Include references to educational resources for complex topics
- Provide context and rationale for rules to facilitate learning

## Remember

- Frontend rules should strike a balance between consistency and allowing for implementation flexibility
- Rules should be living documents that evolve with the project and technology changes
- Focus on guidelines that have the biggest impact on user experience and maintenance
- Include explicit examples that demonstrate the application of each major rule