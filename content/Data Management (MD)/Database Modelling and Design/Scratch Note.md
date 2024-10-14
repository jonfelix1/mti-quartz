Database Modeling and Design

Relational Database Design Methodology
Conceptual database design
◦Step 1 Build conceptual data model
◦ Step 1.1 Identify entitiy types
◦ Step 1.2 Identify relationship types
◦ Step 1.3 Identify and associate attributes with entity or
relationship types
◦ Step 1.4 Determine attribute domain
◦ Step 1.5 Determine candidate, primary, and alternate key
◦ Step 1.6 Consider use of enhanced modelling concepts
◦ Step 1.7 Check model for redundancy
◦ Step 1.8 Validate conceptual data model against user
transactions
◦ Step 1.9 Review conceptual data model with user

Concepts of the ER Model
 Entity types
Group of objects with same properties, identified by
enterprise as having an independent existence:
Physical: Staff, Property, Customer, Part, Supplier, Product
Conceptual: Sale, Course, Inspection.
 Relationship types
Set of meaningful associations among entity types.
Degree of a Relationship
Number of participating entities in relationship: Unary, Binary,
Ternary, Quaternary
 Attributes
Property of an entity or a relationship type.

ER diagram of Branch Has Staff relationship
Unary, Binary, and Ternary Relationship
Multiple Relationship and
Relationship with Attributes

Attributes
 Simple Attribute
 Attribute composed of a single component with an independent
existence.
 Composite Attribute
 Attribute composed of multiple components, each with an
independent existence.
 Multi-valued Attribute
 Attribute that holds multiple values for each occurrence of an entity
type.
 Derived Attribute
 Attribute that represents a value that is derivable from value of a
related attribute, or set of attributes, not necessarily in the same
entity type.

Keys
Candidate Key
◦Minimal set of attributes that uniquely identifies each
occurrence of an entity type.
Primary Key
◦Candidate key selected to uniquely identify each
occurrence of an entity type.
Composite Key
◦A candidate key that consists of two or more attributes.

ER diagram of Staff and Branch entities and
their attributes

Entity Type
Strong Entity Type
◦ Entity type that is not existence-dependent on some other entity type.
Weak Entity Type
◦ Entity type that is existence-dependent on some other entity type.
◦ Dependent entities as rectangles with rounded corners.


Structural Constraints
 Main type of constraint on relationships is called multiplicity.
 Represents policies (called business rules) established by
user or company.
 Multiplicity is made up of two types of restrictions on
relationships: cardinality and participation.
 Cardinality
 Describes maximum number of possible relationship occurrences for
an entity participating in a given relationship type.
 Participation
 Determines whether all or only some entity occurrences participate in
a relationship.

Structural Constraints
The most common degree for relationships is binary.
Binary relationships are generally referred to as being:
◦one-to-one (1:1)
◦one-to-many (1:*)
◦many-to-many (*:*)

Multiplicity of Staff Manages Branch (1:1)
relationship

Multiplicity of Staff Oversees PropertyForRent (1:*)
relationship type

Multiplicity of Newspaper Advertises
PropertyForRent (*:*) relationship

Multiplicity as cardinality and participation
constraints

Enhanced Entity Relationsip
Modelling
Limitations of basic concepts of the ER model
and requirements to represent more complex
applications using additional data modeling
concepts.
Most useful additional data modeling concept of
Enhanced ER (EER) model is called
specialization/generalization.
A diagrammatic technique for displaying
specialization/generalization in an EER diagram
using UML.

The Enhanced Entity-Relationship Model
Since 1980s there has been an increase in
emergence of new database applications with
more demanding requirements.
Basic concepts of ER modeling are not sufficient
to represent requirements of newer, more
complex applications.
Response is development of additional ‘semantic’
modeling concepts.

The Enhanced Entity-Relationship Model
Semantic concepts are incorporated into the
original ER model and called the Enhanced
Entity-Relationship (EER) model.
Examples of additional concept of EER model is
called specialization / generalization.