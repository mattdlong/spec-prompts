You are an expert data architect with extensive experience designing efficient, scalable, and robust data models for software applications across various domains and database technologies.

You have an opportunity to do this work for a very influential billionaire venture capitalist who will accept nothing but the best. If you meet their expectations you will receive fame, fortune, respect and unparalleled credibility, if you fail to meet their expectations you will never work in technology again, your reputation will be ruined, your life will be over.

Your task is to create a comprehensive Data Model Document for the following project:

<data_model_instructions>

{{data_model_instructions}}

</data_model_instructions>

<functional_specifications>

Review the Functional Specification Document at the following location:

"/specifications/FSD.md"

</functional_specifications>

<system_architecture>

Review the System Architecture Document at the following location:

"/specifications/SystemArchitecture.md"

</system_architecture>

<output_instructions>
Output the document to markdown.

Output the document to a subfolder to the root directory named "/specifications".

Name the document DataModel.md.
</output_instructions>

Follow these steps to create the Data Model Document:

<steps>
  
1. Begin with a brief overview explaining the project and the purpose of the document.
  
2. Review the Functional Specification Document and System Architecture Document thoroughly to ensure your data model aligns with the functional requirements and architectural decisions.
  
3. Use sentence case for all headings except for the title of the document, which can be title case.
  
4. Under each main heading include relevant subheadings and fill them with details derived from the provided instructions and previous documents.
  
5. Organize your Data Model Document into the sections as shown in the data_model_outline below.
  
6. For each section, provide detailed and relevant information based on the instructions. Ensure that you:
   - Use clear and concise language
   - Provide specific technical details while explaining complex concepts in an accessible way
   - Maintain consistency throughout the document
   - Address all points mentioned in each section
   - Explicitly reference relevant specifications and architectural decisions from previous documents where appropriate
  
7. When creating the data model:
   - Include text descriptions of all entity-relationship diagrams (as these will be represented in markdown)
   - Define all entities, attributes, relationships, and constraints in detail
   - Document denormalization decisions and their rationale
   - Include data types, lengths, and constraints for all attributes
   - Document indexing strategy and its justification
   - Address data validation, integrity, and consistency requirements
  
8. After completing the Data Model Document, review it against this Final Checklist:
   - Does the data model support all functional requirements identified in the FSD?
   - Are all entities, attributes, and relationships clearly defined?
   - Are appropriate indexes defined to support performance requirements?
   - Has data integrity been properly addressed through constraints and validation rules?
   - Is the model appropriately normalized or denormalized based on requirements?
  
9. Format your Data Model Document:
   - Maintain consistent formatting and numbering
   - Do not use dividers or horizontal rules in the output
   - Format the document in valid Markdown, with no extraneous disclaimers
   - Fix any grammatical errors and ensure proper casing of any names
   - When referring to the project, use simple and conversational language
  
</steps>

<data_model_outline>

# Data Model: {project_title}

## 1. Document information
### 1.1. Document details
   - Bullet list with title, version number, date, and author as different items.
   - Example:
   - **Document title**: Data Model for {project_title}
   - **Version**: 1.0
   - **Date**: {current_date}
   - **Author**: Data Architecture Team

### 1.2. Document purpose
   A brief paragraph explaining the purpose of the Data Model Document and how it provides a blueprint for the data structures that will support the application.

### 1.3. References
   - Bullet list of related documents, with specific references to previously created documents.
   - Example:
   - **Functional Specification Document**: FSD for {project_title}, v1.0
   - **System Architecture Document**: System Architecture for {project_title}, v1.0

## 2. Data architecture overview
### 2.1. Data architecture principles
   - Bullet list of the key principles guiding the data architecture design.
   - Example:
   - **Single source of truth**: Each piece of data should have one authoritative source
   - **Appropriate normalization**: Balance between normalization for data integrity and denormalization for performance
   - **Forward compatibility**: Design should accommodate anticipated future requirements

### 2.2. Database technology selection
   - Bullet list of selected database technologies with justification, referencing the System Architecture Document.
   - Example:
   - **Primary database**: PostgreSQL 13, selected for its robust transaction support, reliability, and feature set
   - **Caching layer**: Redis 6, selected for its performance, versatility, and publish/subscribe capabilities
   - **Search database**: Elasticsearch 7, selected for its full-text search and analytics capabilities

### 2.3. Multi-database strategy (if applicable)
   Description of how multiple databases will be used together, what data will be stored where, and how consistency will be maintained.

## 3. Logical data model
### 3.1. Entity overview
   - Table listing all major entities in the system with brief descriptions.
   - Example:
   
   | Entity | Description |
   |--------|-------------|
   | User | Represents a user of the system with authentication and authorization details |
   | Product | Represents a product in the inventory |
   | Warehouse | Represents a physical location where products are stored |
   | Order | Represents a customer order for products |

### 3.2. Entity-relationship model
   Detailed textual description of the entity-relationship model, including:
   - Entity relationships and cardinality
   - Primary and foreign keys
   - Significant attributes
   
   Include a note that this would typically be represented as an ER diagram in a visual format.

### 3.3. Entity definitions
   For each entity in the system, create a subsection with detailed information:

#### 3.3.1. [Entity name]
   - **Description**: Brief description of what this entity represents
   - **Business key**: Description of the natural or business key, if any
   - **Relationships**: Bullet list of relationships with other entities
     - **Entity**: Relationship type (one-to-many, many-to-many, etc.)
   - **Attributes**: Table of attributes with details
   
   | Attribute | Data Type | Length/Precision | Nullable | Description | Validation Rules |
   |-----------|-----------|------------------|----------|-------------|------------------|
   | id | UUID | N/A | No | Primary key | N/A |
   | name | VARCHAR | 100 | No | User's full name | Min 2 chars, max 100 chars |
   | email | VARCHAR | 255 | No | User's email address | Valid email format |
   | created_at | TIMESTAMP | N/A | No | Record creation timestamp | N/A |

   - **Indexes**: Bullet list of indexes on this entity
     - **idx_user_email**: Unique index on email field for fast lookups and uniqueness enforcement
   - **Constraints**: Bullet list of constraints on this entity
     - **PK_user**: Primary key constraint on id field
     - **UQ_user_email**: Unique constraint on email field

#### 3.3.2. [Next Entity]
   [Same structure as above]

### 3.4. Relationship definitions
   For complex relationships (especially many-to-many), provide detailed descriptions:

#### 3.4.1. [Relationship name]
   - **Entities involved**: List of entities in this relationship
   - **Relationship type**: One-to-one, one-to-many, many-to-many, etc.
   - **Business rules**: Any business rules governing this relationship
   - **Join table details** (for many-to-many): Description of the join table, its attributes, and any constraints

#### 3.4.2. [Next Relationship]
   [Same structure as above]

## 4. Physical data model
### 4.1. Database-specific implementation
   Description of how the logical model maps to the physical implementation in the chosen database(s), including any database-specific features or optimizations.

### 4.2. Denormalization decisions
   - Bullet list of any denormalization decisions made for performance reasons.
   - Example:
   - **Redundant address data**: Customer addresses are stored with orders to preserve historical order information
   - **Aggregated metrics**: Total order value is stored with order to avoid recalculation during reporting

### 4.3. Partitioning strategy
   Description of any table partitioning strategies for large tables, including partition keys and boundaries.

### 4.4. Indexing strategy
   - Bullet list of the overall indexing strategy and specific indexes created for performance.
   - Example:
   - **Selective indexing**: Indexes are created only on columns used in WHERE clauses, JOIN conditions, and ORDER BY clauses
   - **Composite indexes**: Multi-column indexes are used for queries that filter or sort by multiple columns

## 5. Data migration and seeding
### 5.1. Initial data requirements
   - Bullet list of data that needs to be pre-populated in the system.
   - Example:
   - **Lookup data**: Category hierarchies, status codes, and other reference data
   - **Test accounts**: Admin users and test user accounts
   - **Sample data**: Representative sample data for testing and demonstration

### 5.2. Migration strategy
   Description of the approach for migrating data from existing systems, if applicable.

### 5.3. Data quality rules
   - Bullet list of data quality rules to be applied during migration and ongoing operations.
   - Example:
   - **Completeness check**: All required fields must have values
   - **Consistency check**: Related records must maintain referential integrity
   - **Format validation**: Values must conform to specified formats (email, phone, etc.)

## 6. Data access patterns
### 6.1. Common queries
   - Bullet list of common query patterns and how the data model supports them.
   - Example:
   - **User authentication**: Lookup by email with password verification
   - **Product search**: Filter by multiple criteria (category, price range, availability)
   - **Order history**: Retrieve all orders for a specific user with pagination

### 6.2. Data aggregation and reporting
   Description of how the data model supports aggregation and reporting requirements, including any pre-computed aggregates or materialized views.

### 6.3. Caching strategy
   Description of what data will be cached, how it will be invalidated, and how consistency will be maintained.

## 7. Data governance
### 7.1. Data ownership
   Description of how data ownership is defined and managed within the application.

### 7.2. Data lifecycle
   Description of the lifecycle of different types of data, including retention periods and archival policies.

### 7.3. Regulatory compliance
   - Bullet list of regulatory requirements that impact the data model and how they are addressed.
   - Example:
   - **GDPR**: User data is structured to support right to access and right to be forgotten
   - **PCI DSS**: Payment information is tokenized and stored separately with appropriate security controls

## 8. Data security
### 8.1. Access control model
   Description of how data access control is implemented at the database level.

### 8.2. Sensitive data handling
   - Bullet list of how sensitive data is identified and protected.
   - Example:
   - **Encryption at rest**: Sensitive personal data is encrypted in the database
   - **Data masking**: Partial masking of sensitive data in logs and non-production environments
   - **Tokenization**: Payment information is tokenized using a third-party service

### 8.3. Audit logging
   Description of how data changes are logged for audit purposes.

## 9. Performance considerations
### 9.1. Scalability approach
   Description of how the data model supports horizontal and vertical scaling.

### 9.2. Performance optimization techniques
   - Bullet list of techniques used to optimize database performance.
   - Example:
   - **Read replicas**: Separate read and write traffic for better performance
   - **Connection pooling**: Efficiently manage database connections
   - **Query optimization**: Structured queries to make effective use of indexes

### 9.3. Monitoring and tuning
   Description of metrics that should be monitored to identify performance issues and potential tuning approaches.

## 10. Appendices
### 10.1. Glossary
   - Alphabetical list of data-related terms used in the document with definitions.
   - Example:
   - **ACID**: Atomicity, Consistency, Isolation, Durability - properties of database transactions
   - **Normalization**: The process of structuring a database to reduce data redundancy and improve data integrity

### 10.2. SQL scripts
   Description of SQL scripts that will be provided for creating the database schema, including where they will be stored in the project repository.

</data_model_outline>