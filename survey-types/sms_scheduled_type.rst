..  _sms_scheduled_type:

sms_scheduled: Scheduled SMS Survey
=======================================
Text Messages sent on schedule (EMA)

Basic Workflow
-------------------------
* Congigure Survey
* Design Survey Question
* Preview with Dummy Data
* Activate
* Recruit
* Collect

Typical Deployment Configuration
--------------------------------

* 3x/day for 14 days, randomly between participant wake time...

Wave Configuration
------------------------

Go through each screen of the Wave Form or Wizard for a sms_scheduled Wave

Basic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

These are the fields in tab basic

* Name
* Code
* BulkLoadSource
* Notes
* isActive

Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

These are the fields in tab enrollment

* isAutoEnrollOnRegistration
* is_notify_adminstrators
* send_welcome_message
* welcome_message

Workflow
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

These are the fields in tab workflow

* isTracked
* ExternalQueueNames
* IsAutoPopulateData

Expiration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

These are the fields in tab expiration

* survey_expiration
* reminder_frequency
* survey_expiration_response
* warning_frequency
* minimum_break_time
* end_message
* reminder_message
* expiration_message
* warning_message

Extra
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

These are the fields in tab additional


