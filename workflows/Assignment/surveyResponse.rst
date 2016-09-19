Workflow surveyResponse in Assignment
=========================================================

Assignment States
-------------------------------------

* scheduled
* queued
* twilio_error
* initiated
* responding
* abandoned
* complete
* expired

Assignment Transitions
----------------------------------------
#. msg_to_twilio
#. twilio_error
#. direct_message
#. initial_prompt_received
#. never_responds
#. first_response
#. stops_responding
#. all_responses

The Workflow
------------

.. figure::  /images/workflows/surveyResponse.png

   Workflow surveyResponse
