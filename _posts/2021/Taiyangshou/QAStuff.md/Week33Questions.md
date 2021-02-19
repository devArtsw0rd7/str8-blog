Under test coverage? Why, after I have run a test, does it say "NOT RUN" under test coverage?

In a story that I've failed, what does a Requirements Status of NOK (red) mean?

What is the test creation/execution/Jira workflow? How do I(or do I) need to track hours when testing?

Where does BUILD #/Version come into this process? How do I find the build? (This may be related to the fact that I don't have BFFS pulled down correctly yet?)

IN STORY
* Click "Create Test"
  * Project = VBMSTM
  * Issue Type = Test
  * Summary = Default "Test Story Name"
  * Description = Modify if necessary
  * Assignee = Assign to Me
  * Fix Version/Affects Version/s = NOT USED FOR TESTING
  * Priority = Unassigned
  * Attachments = None or Items as needed (for letter templates, I attached the word doc)
  * Labels = Fiduciary (others?)
  * Test Repository Path = Orphans (default)
  * Team = Blank (can't select Taiyangshou for some reason)
  * External Issue ID = NOT USED FOR TESTING
  * Click CREATE
* Back in Story, scroll down to Test Coverage and click on the name of the newly created Test

IN JIRA TEST SCREEN
* Jira Workflow for a Test (What do each of these mean? When do I move from one to the next?)
  * Open
  * Draft
  * Review
  * Approved 
  * Retired
* Execute In button
  * New Test Execution (first time)
    * Pass/Fail Steps
    * 
  * Existing Test Execution (use when retesting a story that initally failed?)



Story
    Linked to a Test
        Open
        Draft
        Review
        Approved
        Retired
            ->Test Execution
                Start Progress
                Stop Progress
                Resolve Issue
                Close Issue

ANSWERED:
When creating tests for our scrum team stories, do we click "Create Test" from the story, or do we still go through VBMSTM (Test Management) and associate our story via the Issues dropdown? CREATE TEST, then select VBMSTM from Projects! (I wasn't added to the project access!)