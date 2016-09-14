
Survey Types
---------------------------------


- **EMA/Personal Surveys**: Collect personal data about participants
- **EMS/Field Surveys**: Collect data about a place, done with field workers
- **Turk Surveys**: Data collected via Mechanical Turk, usually by consensus.


- **Personal Survey Modes** : There are 3 ways to interact with a study participant

 - *SMS*: Text messages.  Each job requires a dedicated phone number, surveys are taken as text messages sent back and forth between the participant and the system, initiated via a *trigger* ( usually random or fixed intervals.)
 - *IVR* : Like SMS, but done with speech and a touch tone phone.
 - *Mobile*: Jobs available via the Survos Mobile app.

- **Field Survey Modes** : There are 3 ways to interact with a field workers:

 - *SMS*: Text messages.  The field worker start the survey by sending a text with an identifier associated with the place being surveyed.
 - *IVR* : Like SMS, but done with speech and a touch tone phone.
 - *Mobile*: Jobs available via the Survos Mobile app.

- **Turk Survey Types** : There are 3 types of Turk surveys:

 - *Consensus*: At least 2 people agree on the answer to a question above some threshold. Additional Turkers do the survey until agreement is reached (Success) or a Turker limit is reached without consensus (Failure).
 - *Expert* : Exactly one worker does the survey task.
 - *Opinion*: Two or more Turkers complete the survey, but there is no expectation on answer agreement.

* **Triggers** : Triggers refer to how a survey is initiated.

 - **Random prompts**: The participant is prompted to take a survey randomly, within certain invervals) during the day.
 - **Fixed prompts**: The participant is prompted with the first survey question either at fixed times.
 - **Self-initiated**: The user initiates the survey, by sending a message (if SMS or MMS), calling a phone number (if IVR) or opening the Survos Mobile app.
 - **Geo-prompted** : If participants are carrying a tracking device, the survey can be triggered when they've been near a location for some time period.
 - **Admin** : used mostly for testing, the administrator can trigger a survey from the dashboard.

- **Participant** : a user is enrolled in a job.  The participant record may contain additional data that is specific to that user's participant in the job, such as their waking hours, or the survey frequency.
- **Dashboard**: The pages on the site where the administrator manages surveys, jobs and users.

Setting Up and Deploying SMS Data Collection
---------------------------------------------

First, you'll create an SMS job, found under the Mobile Jobs menu. which describes *what* you'll be collecting.  Then create the survey questions associated with that job.  Next, enroll yourself in the job and test it.  Then enroll participants in the job, adding them as new users to the system if necessary.

There is also an admin trigger, which is used for testing.  It simply initiates a survey when the administrator triggers it through the dashboard.

Triggers can be mixed, so a survey can be configured to allow self-initiated or done randomly.

Then it's time to recruit some participants.  For the personal version, designed for testing the system and learning survey research, you can post your job to the recruitment page, or you can invite people you know, or you can post a link to a social media site.  (Open for discussion: participant compensation).  The research version allows administrators to enroll participants directly into the system.  This is often done in conjunction with some sort of qualification interview over the phone or in person. The researcher enrollment system allows for anonymous users (often a requirement for survey researcher) and allows for participants to be compensated.

Launch the survey and download your data.

First, create a "mobile job", which describes your study.  These are the types of mobile jobs you can create:
 * SMS: Participants do surveys via an exchange of SMS Messages
 * MMS: Participants collect photos, and possibly some data, using the camera phones and send it to a shortcode.
 * IVR: Participants take surveys via a voice-prompted system, and respond via the touch-pad on their phones.
 * Survos Mobile: Participants download Survos Mobile to their ios or android device, and take the survey on their smartphone.

Creating A Job
-------------------------------------

Choose "Create Job" and select the type of job you want to create.  Because setting up a job has different configuration parameters depending on the type of job it is, you must select the job type first.

All of the job types ask the following information:
 Code
 Title
 Notes
 Type:

   Survos Create Account

Follow the prompts on the screen.  The only item that can't be changed later is the client code, which will also become part of your url, *clientCode*.survos.com.

After a few minutes, you'll receive an email with your account login information.


