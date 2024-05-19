## Introduction to UML

**Definition**: UML (Unified Modeling Language) is a visual language for modeling the structure and behavior of software systems.

**Purpose**: UML helps in planning and visualizing the design of a system, making it easier to understand and communicate ideas.

**Basic UML Diagrams**:
- **Class Diagrams**: Show the static structure of a system.
- **Use Case Diagrams**: Illustrate the interactions between users and the system.
- **Sequence Diagrams**: Detail the order of interactions between objects in a use case.
- **Activity Diagrams**: Represent workflows of stepwise activities.

## Class Diagrams

### Definition

A class diagram depicts the classes in a system and their relationships.

### Components

- **Classes**: Represent entities with attributes and methods.
- **Attributes**: Characteristics of a class.
- **Methods**: Functions or operations a class can perform.
- **Relationships**: Associations between classes, such as inheritance and composition.

### PetClinic Example

Design a simple class diagram for the PetClinic system.
- **Classes**:
    - **Owner**: Attributes - OwnerID, FirstName, LastName, Address, City, Telephone; Methods - addPet(), getPets()
    - **Pet**: Attributes - PetID, Name, BirthDate, Type, OwnerID; Methods - addVisit(), getVisits()
    - **Visit**: Attributes - VisitID, VisitDate, Description, PetID
    - **Vet**: Attributes - VetID, FirstName, LastName; Methods - addSpecialty(), getSpecialties()
    - **Specialty**: Attributes - SpecialtyID, Name

```plaintext
+------------+
|   Owner    |
+------------+
| OwnerID    |
| FirstName  |
| LastName   |
| Address    |
| City       |
| Telephone  |
+------------+
| addPet()   |
| getPets()  |
+------------+

+------------+
|    Pet     |
+------------+
| PetID      |
| Name       |
| BirthDate  |
| Type       |
| OwnerID    |
+------------+
| addVisit() |
| getVisits()|
+------------+

+------------+
|   Visit    |
+------------+
| VisitID    |
| VisitDate  |
| Description|
| PetID      |
+------------+

+------------+
|    Vet     |
+------------+
| VetID      |
| FirstName  |
| LastName   |
+------------+
| addSpecialty() |
| getSpecialties()|
+------------+

+------------+
| Specialty  |
+------------+
| SpecialtyID|
| Name       |
+------------+