Workflow idea:

Create a survey, code, overview, questions, etc.  Choose one or more: "mode": sms, ivr, mining, opinion, mms, etc.  If there are variables, define them here, along with defaults for testing.

From the survey, create one or more "jobs" of this type/mode.  Define the pay, participants, triggers, etc.

Surveys get their own menu.  A job cannot exist without a survey of at least one question.  Sites get sample surveys loaded, but not sample jobs.	

When deploying, use a wizard to deploy the job?

Deployment Mode: 
Triggers
  Random
  Fixed
  Location
  Self

Steps:
Create An Account.
Create/Import a survey
   * Sample Surveys
   * Import from Survey Library (via URL)
   * Create Your Own
   
Should each account have its own library of phone numbers?
Activate this Survey on [Available Phone Numbers]

Ask Twilio: texts received on phones with no url, what happens? Is there a charge?

Design and Launch a one-week SMS Survey With 10 participants for as little as $20!
$5 / week for the phone    5
$1 / week / participant = 10
100 Text Messages   =  $5.

Money Back Guarantee -- Full refund (up to $20) for any reason!

Did you exercise today?
  For how many minutes did you exercise?


Create a Job from the Survey
Add a phone number and Participants
Trigger the survey (need some dynamic updates on the page here)
Review Graphs, Download the Data

Graphs: 
  Pie charts for Radio, Boolean
  Bar Graph for Multiple Choice
  Cloud tag for short text
  
Login with Username/Email/Mobile Phone

Instead of "send password" for mobile phone, could do #register.  Problem, though, is that username, not userId, is used. BAD

Issues: 
username should be userid in ema_participant
jobCode should be jobId

Self-Enrollment


Self-Registration
Your comment has been recorded.  
Create an account by typing in a username and password, like this:
#register username:password <email> 
#turker <turkId>
 / 
MicroPayments at $X dollars paid via paypal

New Job Fields:
	SMS/MMS Automatic Weekly Renewal?
	Renewal Day (of week)
	Prefix for fastadd/anonymous users (e.g. sctc1)
         






