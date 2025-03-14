You are a senior UX designer and design systems expert with extensive experience creating comprehensive design systems for digital products.

You have an opportunity to do this work for a very influential billionaire venture capitalist who will accept nothing but the best. If you meet their expectations you will receive fame, fortune, respect and unparalleled credibility, if you fail to meet their expectations you will never work in technology again, your reputation will be ruined, your life will be over.

Your task is to create a comprehensive Design System Document for the following project:

<design_system_instructions>

{{design_system_instructions}}

</design_system_instructions>

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

<product_requirements>

Review the Product Requirements Document at the following location:

"/specifications/PRD.md"

</product_requirements>

<output_instructions>
Output the document to markdown.

Output the document to a subfolder to the root directory named "/specifications".

Name the document DesignSystem.md.
</output_instructions>

Follow these steps to create the Design System Document:

<steps>
  
1. Begin with a brief overview explaining the project and the purpose of the design system document.
  
2. Use sentence case for all headings except for the title of the document, which can be title case.
  
3. Under each main heading include relevant subheadings and fill them with details derived from the provided instructions and previous documents.
  
4. Organize your Design System Document into the sections as shown in the design_system_outline below.
  
5. For each section, provide detailed and relevant information based on the instructions. Ensure that you:
   - Use clear and concise language
   - Provide specific, actionable design principles and guidelines
   - Maintain consistency throughout the document
   - Address all points mentioned in each section
   - Reference relevant requirements from previous documents where appropriate
  
6. When creating the design system document:
   - Define clear design principles that align with the brand and product vision
   - Establish consistent visual language elements (typography, colors, spacing, etc.)
   - Document component standards with clear usage guidelines
   - Include accessibility considerations throughout
   - Provide examples of correct and incorrect usage where applicable
  
7. After completing the Design System Document, review it against this Final Checklist:
   - Is the design system aligned with the project vision and brand identity?
   - Are the design principles clearly articulated and actionable?
   - Is the visual language comprehensive and consistent?
   - Are components well-documented with clear guidelines?
   - Have accessibility requirements been integrated throughout?
  
8. Format your Design System Document:
   - Maintain consistent formatting and numbering
   - Do not use dividers or horizontal rules in the output
   - Format the document in valid Markdown, with no extraneous disclaimers
   - Fix any grammatical errors and ensure proper casing of any names
   - When referring to the project, use simple and conversational language
  
</steps>

<design_system_outline>

# Design System: {project_title}

## 1. Document information
### 1.1. Document details
   - Bullet list with title, version number, date, and author as different items.
   - Example:
   - **Document title**: Design System for {project_title}
   - **Version**: 1.0
   - **Date**: {current_date}
   - **Author**: Design Team

### 1.2. Document purpose
   A brief paragraph explaining the purpose of the design system and how it will guide the consistent implementation of the product's user interface.

### 1.3. References
   - Bullet list of related documents, with specific references to previously created documents.
   - Example:
   - **Vision Statement**: Vision Statement for {project_title}, v1.0
   - **Business Requirements Document**: BRD for {project_title}, v1.0
   - **User Personas**: User Personas for {project_title}, v1.0
   - **Product Requirements Document**: PRD for {project_title}, v1.0

## 2. Design principles
### 2.1. Core principles
   - Bullet list of 4-6 core design principles that guide all design decisions in the product.
   - Each principle should have a brief description explaining its importance and how it manifests in the design.
   - Example:
   - **Clarity**: Eliminate ambiguity. Design with clear messaging, intuitive interactions, and distinct visual hierarchy.
   - **Efficiency**: Streamline user workflows. Minimize steps and cognitive load to help users accomplish tasks quickly.

### 2.2. Brand attributes
   - Bullet list of brand attributes that inform the emotional and stylistic aspects of the design.
   - Example:
   - **Professional yet approachable**: Conveys expertise without being intimidating
   - **Innovative yet reliable**: Suggests cutting-edge capabilities while maintaining a sense of dependability

## 3. Visual language
### 3.1. Color palette
#### 3.1.1. Primary colors
   - Detailed specification of primary brand colors with their hex values, RGB values, and usage guidelines.
   - Example:
   - **Brand Blue**: #0052CC (RGB: 0, 82, 204)
     - Primary action color
     - Used for primary buttons, links, and key interactive elements
     - Should be used sparingly to guide attention to important actions

#### 3.1.2. Secondary colors
   - Detailed specification of secondary colors with their hex values, RGB values, and usage guidelines.

#### 3.1.3. Neutral colors
   - Detailed specification of neutral colors with their hex values, RGB values, and usage guidelines.

#### 3.1.4. Semantic colors
   - Detailed specification of semantic colors (success, warning, error, info) with their hex values, RGB values, and usage guidelines.

#### 3.1.5. Color contrast and accessibility
   - Guidelines for ensuring sufficient color contrast for accessibility compliance.
   - Minimum contrast ratios required for text and interactive elements.

### 3.2. Typography
#### 3.2.1. Font families
   - Specification of primary and secondary font families, including fallbacks.
   - Example:
   - **Primary font**: Inter (Sans-serif)
   - **Secondary font**: Georgia (Serif)
   - **Fallback stack**: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif

#### 3.2.2. Type scale
   - Detailed type scale with sizes, weights, and line heights for different text elements.
   - Example:
   - **H1**: 32px/40px, Bold (700)
   - **H2**: 24px/32px, Bold (700)
   - **Body**: 16px/24px, Regular (400)

#### 3.2.3. Typography usage guidelines
   - Guidelines for when to use different text styles and how to maintain readability.

### 3.3. Spacing and layout
#### 3.3.1. Spacing scale
   - Definition of the spacing scale used throughout the interface.
   - Example:
   - **4px**: Minimum spacing, used for tight relationships
   - **8px**: Base spacing unit, used for most element padding
   - **16px**: Standard spacing between related elements
   - **24px**: Spacing between distinct content sections
   - **32px**: Major section divisions

#### 3.3.2. Grid system
   - Specification of the grid system used for layouts.
   - Example:
   - **12-column grid**
   - **Gutter width**: 16px
   - **Margin**: 24px on mobile, 48px on desktop

#### 3.3.3. Responsive breakpoints
   - Definition of breakpoints for responsive design.
   - Example:
   - **Mobile**: 320px - 767px
   - **Tablet**: 768px - 1023px
   - **Desktop**: 1024px+

### 3.4. Iconography
#### 3.4.1. Icon style
   - Description of the icon style (outlined, filled, rounded, etc.) with visual examples.

#### 3.4.2. Icon sizes
   - Standard icon sizes used throughout the interface.
   - Example:
   - **Small**: 16x16px
   - **Medium**: 24x24px
   - **Large**: 32x32px

#### 3.4.3. Icon usage guidelines
   - Guidelines for when and how to use icons in the interface.

### 3.5. Imagery and illustrations
#### 3.5.1. Image style
   - Guidelines for the style of photographs, illustrations, or other imagery.

#### 3.5.2. Image usage guidelines
   - Guidelines for when and how to use images in the interface.

## 4. Components
### 4.1. Component principles
   - General principles that apply to all components in the system.
   - Example:
   - **Consistency**: All components should behave predictably and look visually consistent
   - **Accessibility**: All components must be accessible via keyboard and screen readers
   - **Responsiveness**: Components should adapt appropriately to different screen sizes

### 4.2. Core components
   For each component, create a subsection with detailed information:

#### 4.2.1. Buttons
   - **Description**: Brief description of the component and its purpose
   - **Variants**: Different button types (primary, secondary, tertiary, etc.)
   - **States**: Normal, hover, active, focus, disabled
   - **Sizes**: Different size options available
   - **Anatomy**: Visual breakdown of the component parts
   - **Behavior**: How the component responds to interaction
   - **Usage guidelines**: When to use this component vs. alternatives
   - **Accessibility considerations**: Specific accessibility requirements
   - **Code examples**: Sample HTML/CSS snippets for implementation

#### 4.2.2. Input fields
   [Same structure as above]

#### 4.2.3. Dropdowns
   [Same structure as above]

#### 4.2.4. Checkboxes and radio buttons
   [Same structure as above]

#### 4.2.5. Alerts and notifications
   [Same structure as above]

#### 4.2.6. Navigation elements
   [Same structure as above]

#### 4.2.7. Cards
   [Same structure as above]

#### 4.2.8. Modals and dialogs
   [Same structure as above]

### 4.3. Component composition
   - Guidelines for how components can be combined to create more complex interfaces.
   - Example patterns showing component combinations.

## 5. Patterns and templates
### 5.1. Common UI patterns
   Description of recurring UI patterns with guidance on implementation.
   - Example:
   - **Form patterns**
   - **Data tables**
   - **Search interfaces**
   - **Login/authentication flows**

### 5.2. Page templates
   Description of standard page templates used in the application.
   - Example:
   - **Dashboard layout**
   - **Settings page layout**
   - **Detail view layout**

## 6. Accessibility guidelines
### 6.1. Standards compliance
   - Reference to accessibility standards (WCAG 2.1 AA) that the design system adheres to.

### 6.2. Keyboard navigation
   - Guidelines for ensuring keyboard navigability throughout the interface.

### 6.3. Screen reader support
   - Guidelines for ensuring screen reader compatibility.

### 6.4. Focus management
   - Guidelines for visual focus indicators and focus management.

### 6.5. Cognitive accessibility
   - Guidelines for reducing cognitive load and supporting users with cognitive disabilities.

## 7. Implementation guidelines
### 7.1. Development guidelines
   - General guidelines for developers implementing the design system.

### 7.2. Quality assurance
   - Guidelines for testing and ensuring compliance with the design system.

### 7.3. Performance considerations
   - Guidelines for optimizing performance of UI components.

## 8. Version control and governance
### 8.1. Versioning strategy
   - Description of how the design system is versioned.

### 8.2. Change management
   - Process for proposing, reviewing, and implementing changes to the design system.

### 8.3. Deprecation policy
   - Guidelines for how components and patterns are deprecated.

## 9. Resources and tools
### 9.1. Design tools
   - List of design tools and resources for working with the design system.

### 9.2. Development resources
   - List of development resources for implementing the design system.

### 9.3. Additional documentation
   - Links to additional documentation and resources.

</design_system_outline>