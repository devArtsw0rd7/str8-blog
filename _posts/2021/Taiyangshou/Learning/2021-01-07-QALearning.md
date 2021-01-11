# Advanced Testing Concepts

## Black Box Testing

### **Types of Black Box Testing**
#### Equivalence Partitioning (Equivalence Class Partitioning)
    * This can be applied to all levels of testing (Unit, Integration, System, etc.)
    * **Definition:** Eliminating the set of input data that make the system behave the same and yield the same result when testing an application. repetitive/redundant test cases.
    * **Goal:** Eliminate 
    * **Rationale:** Rather than testing all possible values in a test condition, the possible values of tickets are divided into groups where the system behavior can be considered the same. *If one condition/value in a partition passes/fails, then all others will also pass/fail.*
    * **Info:** 
        * The divided sets are known as *Equivalence Classes/Equivalence Partitions* 
        * Only one value from each partition is selected for testing
#### Boundary Value Analysis (Range Checking)
    * Complimentary to Equivalence Partitioning and can be applied to all levels of testing
    * **Definition:** Testing the boundary values between equivalence partitions.
    * **Goal:** Identify errors at boundaries.
    * **Rationale:** Extreme ends of the input domain can cause more errors in a system.
    * **Upshot:** 3 tests for each boundary (below, on, above boundary) 
    * **Typical Use:** In conjunction with Equivalence Partitioning
    
#### Decision Table Testing
    * A good way to record complex business rules that a system must implement
    * Allows testers to search the effects of combinations of different inputs and other software states that must correctly implement business rules
    * 
#### State Transition Testing
#### Use Case Testing

