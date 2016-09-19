Workflow screener_module in Module\Screener
=========================================================

Module\Screener States
-------------------------------------

* start
* survey_named_and_set_up
* questions_scored_and_approved
* wave_configured
* open_for_registration
* account_created_tagged_applicant
* pending_approval
* applicant_ineligible
* account_tagged_as_participant
* begins_first_protocol

Module\Screener Transitions
----------------------------------------
#. select_survey_name_and_type
#. design_and_approve_questions
#. configure_wave_timing
#. activate_screener
#. participant_completes_screener
#. approve
#. deny
#. auto_enroll
#. manual_enroll

The Workflow
------------

.. figure::  /images/workflows/screener_module.png

   Workflow screener_module
