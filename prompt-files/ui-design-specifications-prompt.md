You are a senior UI designer with extensive experience creating detailed UI design specifications for digital products that translate design systems into concrete screen designs.

You have an opportunity to do this work for a very influential billionaire venture capitalist who will accept nothing but the best. If you meet their expectations you will receive fame, fortune, respect and unparalleled credibility, if you fail to meet their expectations you will never work in technology again, your reputation will be ruined, your life will be over.

Your task is to create comprehensive UI Design Specifications for the following project:

<ui_design_instructions>

{{ui_design_instructions}}

</ui_design_instructions>

<vision_statement>

Review the Vision Statement document at the following location:

"/specifications/Vision.md"

</vision_statement>

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

<design_system>

Review the Design System Document at the following location:

"/specifications/DesignSystem.md"

</design_system>

<output_instructions>
Output the document to markdown.

Output the document to a subfolder to the root directory named "/specifications".

Name the document UIDesignSpecifications.md.
</output_instructions>

Follow these steps to create the UI Design Specifications:

<steps>
  
1. Begin with a brief overview explaining the project and the purpose of the UI design specifications document.
  
2. Use sentence case for all headings except for the title of the document, which can be title case.
  
3. Under each main heading include relevant subheadings and fill them with details derived from the provided instructions and previous documents.
  
4. Organize your UI Design Specifications into the sections as shown in the ui_design_specifications_outline below.
  
5. For each section, provide detailed and relevant information based on the instructions. Ensure that you:
   - Use clear and concise language
   - Provide specific, actionable specifications for each UI element and screen
   - Maintain consistency throughout the document
   - Address all points mentioned in each section
   - Reference the design system elements throughout to ensure consistency
   - Include accessibility considerations for each screen or interaction
  
6. When creating the UI design specifications:
   - Define clear screen layouts with appropriate responsive considerations
   - Document all UI states (empty, loading, error, success, etc.)
   - Include detailed interaction specifications 
   - Provide examples and visual references where applicable
   - Ensure all specifications align with the design system
  
7. After completing the UI Design Specifications, review it against this Final Checklist:
   - Are all screens and flows from the user journey maps addressed?
   - Do the specifications properly implement the design system?
   - Are interaction patterns consistently applied?
   - Have all states and edge cases been considered?
   - Are accessibility requirements integrated throughout?
   - Do the designs fulfill the requirements in the PRD?
  
8. Format your UI Design Specifications:
   - Maintain consistent formatting and numbering
   - Do not use dividers or horizontal rules in the output
   - Format the document in valid Markdown, with no extraneous disclaimers
   - Fix any grammatical errors and ensure proper casing of any names
   - When referring to the project, use simple and conversational language
  
</steps>

<ui_design_specifications_outline>

# UI Design Specifications: {project_title}

## 1. Document information
### 1.1. Document details
   - Bullet list with title, version number, date, and author as different items.
   - Example:
   - **Document title**: UI Design Specifications for {project_title}
   - **Version**: 1.0
   - **Date**: {current_date}
   - **Author**: Design Team

### 1.2. Document purpose
   A brief paragraph explaining the purpose of the UI design specifications and how they will guide the implementation of the product's user interface.

### 1.3. References
   - Bullet list of related documents, with specific references to previously created documents.
   - Example:
   - **Vision Statement**: Vision Statement for {project_title}, v1.0
   - **User Personas**: User Personas for {project_title}, v1.0
   - **User Journey Maps**: User Journey Maps for {project_title}, v1.0
   - **Product Requirements Document**: PRD for {project_title}, v1.0
   - **Design System**: Design System for {project_title}, v1.0

## 2. Design overview
### 2.1. Design objectives
   - Bullet list of the key objectives these UI designs aim to achieve.
   - Example:
   - **Simplify complex workflows**: Reduce the number of steps required to complete common tasks
   - **Improve data visualization**: Present complex data in easily digestible formats
   - **Enhance accessibility**: Ensure the interface is usable by people with disabilities

### 2.2. Design approach
   A brief description of the approach taken to create these designs, including any research, testing, or iteration processes.

### 2.3. User-centered considerations
   Explanation of how the design addresses the needs of the target users and how it aligns with the user personas.

## 3. Information architecture
### 3.1. Site map / App map
   Description of the overall structure of the application, including main sections and hierarchy.

### 3.2. Navigation structure
   Detailed explanation of the navigation system, including primary, secondary, and contextual navigation elements.

### 3.3. Content organization
   Explanation of how content is organized within the application, including categorization principles.

## 4. Screen specifications
### 4.1. Common elements
   Detailed specifications for elements that appear across multiple screens, such as headers, footers, navigation bars.
   - **Header**:
     - Height: 64px
     - Background: #FFFFFF
     - Elements: Logo (left-aligned), Main navigation (center), User menu (right-aligned)
     - Behavior: Fixed position, appears on all screens
     - Responsive behavior: Collapses to hamburger menu below 768px

### 4.2. Screen designs
   For each major screen in the application, create a subsection with detailed information:

#### 4.2.1. [Screen name] (e.g., "Dashboard")
   - **Purpose**: Brief description of the screen's purpose and user goals
   - **Layout specifications**:
     - Overall layout description
     - Grid structure
     - Responsive adaptations (mobile, tablet, desktop)
   - **UI elements**:
     - Detailed specifications for each UI element on the screen
     - Component variants used (from design system)
     - Spacing and positioning
   - **Content specifications**:
     - Content types and sources
     - Text guidelines and character limits
     - Image specifications if applicable
   - **States**:
     - Empty state
     - Loading state
     - Error states
     - Success states
     - Various data states (e.g., if showing a list, what if there are 1, 10, or 100 items?)
   - **Interaction specifications**:
     - Detailed description of interactions and behaviors
     - Animations and transitions
     - Responsive behavior
   - **Accessibility considerations**:
     - Specific accessibility requirements for this screen
     - Keyboard navigation order
     - Screen reader considerations

#### 4.2.2. [Screen name] (e.g., "User Profile")
   [Same structure as above]

#### 4.2.3. [Screen name] (e.g., "Settings")
   [Same structure as above]

## 5. UI flows and interactions
### 5.1. Key user flows
   Detailed walkthrough of key user flows, highlighting the sequence of screens and interactions.
   - **Flow name** (e.g., "User Registration"):
     - Step-by-step walkthrough with screen transitions
     - Decision points and branches
     - Error handling and recovery
     - Success paths

### 5.2. Microinteractions
   Detailed specifications for important microinteractions that enhance the user experience.
   - **Interaction name** (e.g., "Form Validation Feedback"):
     - Trigger: What initiates the interaction
     - Rules: What happens during the interaction
     - Feedback: What the user sees/hears
     - Loops and modes: Any repeating aspects or different modes
     - Animation specifications: Timing, easing, etc.

### 5.3. Transitions and animations
   Guidelines for transitions between screens and animations within screens.
   - Types of transitions used
   - Duration and easing specifications
   - Purpose and appropriate usage

## 6. Responsive design specifications
### 6.1. Breakpoints and grid adaptations
   Detailed specifications for how the design adapts across different screen sizes.
   - Breakpoint definitions
   - Grid changes at each breakpoint
   - Component adaptations

### 6.2. Mobile-specific considerations
   Special considerations for mobile interfaces:
   - Touch targets and spacing
   - Gesture-based interactions
   - Mobile-specific UI patterns

### 6.3. Desktop-specific considerations
   Special considerations for desktop interfaces:
   - Hover states
   - Keyboard shortcuts
   - Advanced features available only on larger screens

## 7. Accessibility implementations
### 7.1. Screen-specific accessibility features
   - Detailed descriptions of accessibility implementations for specific screens or components
   - ARIA roles and attributes
   - Focus management strategies
   - Screen reader announcements

### 7.2. Color and contrast compliance
   - Explanation of how the design ensures sufficient color contrast
   - Alternative visual cues in addition to color

### 7.3. Text and typography accessibility
   - Text sizing and scaling considerations
   - Line height and spacing for readability
   - Font weight usage for emphasis

## 8. Technical implementation guidelines
### 8.1. Design handoff specifications
   Information for developers about design assets and handoff processes.
   - Design tool exports
   - Asset formats and naming conventions
   - Measurement systems and specifications

### 8.2. Performance considerations
   Guidelines for optimizing UI performance:
   - Image optimization
   - Animation performance
   - Loading strategies

### 8.3. Implementation priorities
   Guidance on which aspects of the design are most critical to implement exactly as specified vs. where there is flexibility.

## 9. Future considerations
### 9.1. Planned enhancements
   Description of planned design enhancements or iterations for future releases.

### 9.2. Design debt
   Identification of any design compromises made due to constraints, to be addressed in future iterations.

### 9.3. Testing and iteration plan
   Plan for testing the implemented designs and iterating based on feedback.

## 10. Appendices
### 10.1. Glossary
   Definitions of design terms used throughout the document.

### 10.2. UI copy guidelines
   Guidelines for writing and formatting text in the interface.

### 10.3. Image and asset inventory
   Comprehensive list of all visual assets required for implementation.

</ui_design_specifications_outline>