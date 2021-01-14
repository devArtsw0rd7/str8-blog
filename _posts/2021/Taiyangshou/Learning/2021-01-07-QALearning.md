# Advanced Testing Concepts

## Black Box Testing
    * Testing in which the tester does not know the internal implementation of a function (internals not visible)
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
  
    * To determine the number of test cases:
      * 2 = 2^n
      * So, for 3 conditions, it would be 2^3 = 8 cases
#### State Transition Testing
    * Shows all valid transitions and potentially invalid transitions between states, as well as the events, guard conditions, and resulting actions for valid transitions
    * This technique is used when features of a system are represented as states which transform one another.
    * State charts help understand all possible flows
    * WHEN TO USE: 
      * sequence of events need to be tested
      * an application is dependent upon the event/values/conditions of the past (x before y)
#### Use Case Testing
    * a black-box testing technique to help testers write better test cases in order to increase the quality of the software
    * Each use case specifies some behavior that a subject can perform in collaboration with one or more actors
    * Typically used in Agile Framework
      * Actors, steps, description, system, extension

"O-switch coverage"- every single transition in a system is tested
    * # of cases = # of transitions (arrows in the diagram)

"1-switch coverage"- every two pair transition in a system is tested

#### Negative Testing
    * Proper test coverage includes positive and negative testing
    * Positive testing = determines that the application works as expected ("Happy Path" testing)
    * Negative testing = ensures that an application can gracefully handle invalid input or unexpected user behavior
    * PURPOSE: detect such unexpected situations and prevent the app from crashing


    Common examples: populating required fields (make a test that leaves required fields empty)
                     allowed data bounds and limits (tests outside of accepted limits)

#### Smoke, Sanity, and Regression Testing

    * Smoke Testing (Initial unstable builds)
      * carried out during initial development stages of the SDLC to make sure core functionalities of a program are working fine without any issues
      * Main tenet: Verify that the core or main functionalities work (NOT DEEP TESTING)
    * Done when developers provide a fresh build to the QA team or when a new module is added to existing functionality

    * Sanity Testing (Stable builds- Surface level testing to figure out if software is ready for end-to-end testing)
      * performed to check whether a software product is working correctly when a new module or functionality gets implemented to an existing product
      * usually performed after receiving a stable software build or after minor changes in code/functionality
      * Typically performed after a bug fix, just before deployment to prod


    * Regression testing (Complete Verification testing)
      * Any time production code is changed
      * the process of verifying that the software still performs correctly after changes were introduced
      * ensures enhancements or bug fixes have not adversely affected what was previously built and tested
      * new tests are not created, but previous tests are re-run

        * Promotes the improvement of product quality
        * ensures that issues already detected and fixed are not recreateable
        * allows dev team to be confident about the release

#### Risk-based testing

    * helps prioritize testing to obtain higher levels of quality
    * Risk = Impact x Likelihood


#### Static & Dynamic Testing
    * Dynamic Testing
      * Requires software to be executed 
    * Static Testing
      * assess code or work product 

#### Test Plan
    * document detailing objectives, resources, and processes for a specific test
      * What to test?
      * How to test?
      * How much time?


