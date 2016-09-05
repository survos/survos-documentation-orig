Enrolling Members by Text
==============================

These are the ways for people to become members of a project.  A project member is _anyone_ who touches the project
in any way: the project owner, managers, collaborator, and of course the cohort itself and the applicants.

* A manager can invite someone to join
* A manager can add someone to the cohort, but not as a researcher (since researchers must have their own Survos account)
* A person can apply to join via the web
* A person can apply to join by sending a specially-formatted text message


Self-Enrollment via Text
------------------------

# A project must purchase a text message number by going to the Twilio tab and choose "Buy A New Number".
# Associate this number with the project (Edit project, etc.)
# Now the registration page (http://unc.l.survos.net/app_dev.php/register/) will say

   You can also register by texting
       #register email
    to (919) 883-4574, where email is your email address.

# When the text message is received, a new member record is created (or updated, if either the email or phone number
already exists in the member, aka ProjectUser, table.  If new, it uses a default member code, which is defined in the project.
A text message response is sent to the user with the member code and status, based on what is set in the project.

Example messages include
   "Your member identifier is unc0014.  Complete your registration and download the Survos app by following the instructions sent to <email>."
   "You have successfully enrolled in morning_coffee_sms, you will receive 3 random text prompts between 9AM and 11AM"
   "If your current time is not 3:34PM, respond to this text with #time 4:34PM (or whatever the local time was)"

(We could also require the time when registering, e.g. "#register <email> 3:34PM")

If the phone number matches a USER account, then that user is associated with the phone number.  (Since e-mails can be spoofed or mis-typed,
we may want to handle those differently).

The email sent to the new member, containing links to register and download the app.  The registration link in the email
includes an invitation code associated with the member (in the ProjectUser table), so that the new user record can
be immediately associated with the member record, and also to pre-fill the email field on the registration form.

Adding Participants to a Job
----------------------------

(TEXT and screenshots here)

Enrolling A User from User Profile Page
---------------------------------------

(text and screenshots)

Enrolling a Participant
^^^^^^^^^^^^^^^^^^^^^^^

1. Install CHAT app

   * iPhone: [insert instructions]
   * Android: [insert instructions]

2. Add new user to Survos

   * Click “participants” on left-hand column

   * Click “Create new user”

   * Enter their mobile phone #!!!

   * Enter user name (same as baseline ID number)

   * Enter password (same as user name)

   * Click “save”

   * Click “Add new device”

   * Enter their chat number and click on the search button

   * Select “chat-iOS” for type

   * Click “save”

3. Enroll participant

   * Click on the “random” study

   * Click on the “enrollees” tab

   * Click “add new participant”

   * Select the user by clicking on the box to the left of their name/id

   * Enter the start date (if left blank it will start today)

   * “Verbosity” – choose “normal”

   * Click “ADD”

   * Go back to the home page

   * Click on “cig” study

   * Click on the “enrollees” tab

   * Click “add new participant”

   * Select the user by clicking on the box to the left of their name/id

   * Enter start date

   * Verbosity – normal

   * Click add

4. Send test survey

   * Click on the “random” study

   * Click on the “enrollees” tab

   * Select the box to the left of the participant’s user name

   * Action > Initiate Right now

   * Click “Do action”

5. Schedule survey

   * Click on the “cig” study

   * Click on the “enrolles” tab

   * Select the box to the left of the participant’s user name

   * Click on the pencil icon

   * Enter start date

   * Enter number of days: 7

   * Verbosity: normal

   * Frequency: 6

   * Enter start and end time (8 hours)

   * Click submit”

6. Program phone numbers into participants phone

   * 202-688-0658 “Cig Survey”

   * 202-601-3699 “Random Survey”

7. Explain incentives

   * Give them a copy of the incentives chart
