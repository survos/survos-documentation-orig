..  _ivr_self_report_type:

ivr_self_report: Self Report via IVR Survey
=======================================
Calls initiated by participant (IVR)

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

Go through each screen of the Wave Form or Wizard for a ivr_self_report Wave

Basic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _tab_url: basic http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=ivr_self_report#basic

These are the fields in tab basic.   This is what it should look like: basic_.


.. image:: http://dummyimage.com/600x400/000/fff&text=ivr_self_report+Wave+Tab+basic
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form ivr_self_report Wave Tab basic

* Name
* Code
* BulkLoadSource
* Notes
* isActive

Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _tab_url: enrollment http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=ivr_self_report#enrollment

These are the fields in tab enrollment.   This is what it should look like: enrollment_.


.. image:: http://dummyimage.com/600x400/000/fff&text=ivr_self_report+Wave+Tab+enrollment
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form ivr_self_report Wave Tab enrollment

* isAutoEnrollOnRegistration
* is_notify_adminstrators

Workflow
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _tab_url: workflow http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=ivr_self_report#workflow

These are the fields in tab workflow.   This is what it should look like: workflow_.


.. image:: http://dummyimage.com/600x400/000/fff&text=ivr_self_report+Wave+Tab+workflow
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form ivr_self_report Wave Tab workflow

* isTracked
* ExternalQueueNames
* IsAutoPopulateData

