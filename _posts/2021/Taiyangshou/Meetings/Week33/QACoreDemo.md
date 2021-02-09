# QA Core Demo
## Monday, February 8th, 2021

VBMS Core for Testers
* Veteran Profile
* Claims
* Letters
* Package Manager
* Exam Management
* Accounts per role

# Q: Is there a list of existing users?
# Q: List of Roles?

350
ISQA350_SSUPER9

Station 350

IF system outage:
    Report in slack

Default Screen = Work Queue
List of Claims

Click RO 350 (VSRs click here to see what they need to work on)

# Q: How do we know which user to use for a particular test?

Enter veteran File# to search for it

# Q: Test for all users? How do you know which users you need to test for? In the story? 

EOD: Entry on Duty
RAD: Release from Active Duty

In order to rate/award a Vet, they must have a verified Service
* Character of Discharge- Honorable
* Separation- Satisfactory
* Verified- Yes
* Save

SSN- start with 999 or 666


SMOKE TEST
Action dropdown
* New Claim

Claim Establishment Screen
* EP&Claim Label- 400/020NEW
* Modifier (For certain claims, there are 10 modifiers...you can only do 10 of the same type of claim!!!!)

* Date of Claim (today's date)
* Segmented lane-> just pick one
* Station-> 499 (NWQ)
* Contact Info
  * Address (TEST)
  * City (TEST)
  * State (SC)
  * Zip (29464)
Address Suggestion-> Use address

CLAIMS SCREEN
* Need contentions to do letters, exams, etc.
* Add Contentions (Free text field) Contention1, Contention2, etc.
* Classification (must pick from the list-> depending on testing, you may need to pick something specific, otherwise pick whatever...hearing loss, etc.)


WHEN YOU FIND SOMETHING THAT IS SUPPOSED TO HAPPEN AND DOESN'T, MAKE A NOTE OF IT, YOU MAY HAVE JUST FOUND A BUG!!!

Check if something is down in the system if things start breaking...

My History-> List of Claims you've been looking at

## Letters (Chevron at top of claim)
Generate correspondence sent out to a veteran

Certain letters require certain contentions

USE A GENERIC LETTER TO TEST
* Custom 5103 Notice
* Add letters button
* Edit letter screen (as needed)
* Salutation
* Associated Development Actions
  * Standard VSO notice (for example)
* Standard Enclosures
* Preview Letter (will show a DRAFT until finalized)
* Checking the Preview is a Test to see that everything is there

Finalize Letter
* Claim Check (issues that are needed...may be ok if not testing those things)
* Acknowlegde
* Finalize
* Proceed and ignore warnings

Status should now be Finalized

NEXT IN THE CLAIMS PROCESS-> Package Manager (Pac Man) Veteran Drop down
* Takes all documents generated, and packages them up, sends them to a central location, processed, printed, and sent out
* Date Sent (should always be the next business day after the Finalized date)
  

Add Documents
* eFolder
* Standard Enclosures

CLICK SAVE AFTER ADDING DOCUMENTS!!!

Send Package
Main screen = Success

EXAM
* Exam being requested related to the contention

WHEN TESTING EXAMS:
Gear icon-> Check Use Exam Destination Mock Data (check box)
Allows you to simulate 3rd party data

Create new request

1. Select contention
2. Claim Information (edit as needed...addd a Veteran Geo location, POA, etc.)
3. Contentions

DBQ=Disability Benefit Questionnaire

(System should help by highighting in yellow the DBQ you need)
Click arrow to move it over to Selected

4. Preview ESR (PDF of Exam Scheduling Request)

Verify all info you expect to see
All 4 boxes are checked and green

SUBMIT ESR
* Exam Destination
  * Mock data check button allows you to select alternate destinations
  * Select Test Double
  * Justification
  * Explanation
  * Preview PDF again to check exam request destination
  * Submit button

Under Exams you should now see exam requests (clicking the Newspaper icon allows you to see specific data ... UUID, etc.)

Under Vendor- Test on VAS (Vendor Action System)
## Design New Action (How to know which one to pick? Based on specific test?)
* Action Type
  * Ackknowlege
  * Clarification Request
    TO VBMS
        * Actions->History
        * Click on Letter with Red !
        * Respond to the clarification in VBMS (required fields...put whatever)
        * 
  * Create APpointment
  * Complete Appointment
  * Results package available

ADD TO QUEUE, then SUBMIT

Close out all Tracked items (Add Closed Date) before going to Ratings



