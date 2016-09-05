... This file was automatically generated from SCRIPT_NAME -- do not modify it except to change the relevant twig file!

..  _sms_single_type:

sms_single: One-time SMS Survey
=======================================
Welcome message, Phone verification code

Basic Workflow
-------------------------
* Configure a One-time SMS Survey
* Design Survey Questions
* Preview with Dummy Data
* Activate
* Recruit
* Collect

Typical Deployment Configuration
--------------------------------

* 3x/day for 14 days, randomly between participant wake time...

Wave Configuration
------------------------

Go through each screen of the Wave Form or Wizard for a sms_single Wave

Basic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _tab_url: basic http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=sms_single#basic

These are the fields in tab basic.   This is what it should look like: tab_url_.


.. image:: http://dummyimage.com/600x400/000/fff&text=sms_single+Wave+Tab+basic
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form sms_single Wave Tab basic

* Name
* Code
* BulkLoadSource
* Notes
* isActive

Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _tab_url: enrollment http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=sms_single#enrollment

These are the fields in tab enrollment.   This is what it should look like: tab_url_.


.. image:: http://dummyimage.com/600x400/000/fff&text=sms_single+Wave+Tab+enrollment
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form sms_single Wave Tab enrollment

* isAutoEnrollOnRegistration
* is_notify_adminstrators
* send_welcome_message
* welcome_message

Workflow
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _tab_url: workflow http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=sms_single#workflow

These are the fields in tab workflow.   This is what it should look like: tab_url_.


.. image:: http://dummyimage.com/600x400/000/fff&text=sms_single+Wave+Tab+workflow
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form sms_single Wave Tab workflow

* isTracked
* ExternalQueueNames
* IsAutoPopulateData

Expiration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _tab_url: expiration http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=sms_single#expiration

These are the fields in tab expiration.   This is what it should look like: tab_url_.


.. image:: http://dummyimage.com/600x400/000/fff&text=sms_single+Wave+Tab+expiration
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form sms_single Wave Tab expiration

* survey_expiration
* reminder_frequency
* survey_expiration_response
* warning_frequency
* minimum_break_time
* end_message
* reminder_message
* expiration_message
* warning_message

