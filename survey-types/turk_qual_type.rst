... This file was automatically generated from SCRIPT_NAME -- do not modify it except to change the relevant twig file!

..  _turk_qual_type:

turk_qual: Turk Qualifications Survey
=======================================
Internal, used for storing Turk Qualification Tasks

Basic Workflow
-------------------------
* Configure a Turk Qualifications Survey
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

Go through each screen of the Wave Form or Wizard for a turk_qual Wave

Basic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _tab_url: basic http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=turk_qual#basic

These are the fields in tab basic.   This is what it should look like: tab_url_.


.. image:: http://dummyimage.com/600x400/000/fff&text=turk_qual+Wave+Tab+basic
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form turk_qual Wave Tab basic

* Name
* Code
* BulkLoadSource
* Notes
* isActive

Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _tab_url: enrollment http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=turk_qual#enrollment

These are the fields in tab enrollment.   This is what it should look like: tab_url_.


.. image:: http://dummyimage.com/600x400/000/fff&text=turk_qual+Wave+Tab+enrollment
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form turk_qual Wave Tab enrollment

* isAutoEnrollOnRegistration
* is_notify_adminstrators

Workflow
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _tab_url: workflow http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=turk_qual#workflow

These are the fields in tab workflow.   This is what it should look like: tab_url_.


.. image:: http://dummyimage.com/600x400/000/fff&text=turk_qual+Wave+Tab+workflow
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form turk_qual Wave Tab workflow

* isTracked
* ExternalQueueNames
* TurkDeployment
* IsAutoPopulateData

Qualifications
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _tab_url: qualifications http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=turk_qual#qualifications

These are the fields in tab qualifications.   This is what it should look like: tab_url_.


.. image:: http://dummyimage.com/600x400/000/fff&text=turk_qual+Wave+Tab+qualifications
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form turk_qual Wave Tab qualifications

* HitTitle
* HitDescription
* HitAnnotation
* TestDurationInSeconds
* RetryDelayInSeconds
* HitKeywords
* ProcessMethod
* IsAutoGrant
* DefaultScore

