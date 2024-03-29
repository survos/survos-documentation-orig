.. This file was automatically generated from SCRIPT_NAME -- do not modify it except to change the relevant twig file!

<<<<<<< HEAD
..  _WebInterview_integration_type:

WebInterview Integration Types
=======================================
WebInterview

The purpose of this integration is to provide a channel to collect data.

=======
..  _WebInterview_type:

WebInterview Surveys
=======================================
WebInterview

Basic Workflow
-------------------------
* Configure a WebInterview Survey
* Design Survey Questions
* Preview with Dummy Data
* Activate
* Recruit
* Collect

Typical Deployment Configuration
--------------------------------

* 3x/day for 14 days, randomly between participant wake time...
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d

WebInterview Wave Configuration
------------------------

Go through each screen of the Wave Form or Wizard for a WebInterview Wave

WebInterview Basic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `basic Tab in the WebInterview Wave
<http://behattest.stagingsurvos.com/waves/dummy/WebInterview#basic>`_.

.. figure::  /images/modules/ongoing_WebInterview_basic.png

   Rendered Form WebInterview Wave Tab basic

.. raw:: html

    <div class="wy-table-responsive">
    <table border="1" class="docutils">
        <colgroup>
        <col width="15%">
        <col width="25%">
        <col width="60%">
        </colgroup>
        <thead valign="bottom">
            <tr class="row-odd">
                <th class="head">Field</th>
                <th class="head">Info</th>
                <th class="head">Description</th>
            </tr>
        </thead>
        <tbody valign="top">
                                    <tr class="row-odd">
                <th class="head">
                    Name                </th>
                <td>
                                            <b>Type</b>: string(80)                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Code                </th>
                <td>
                                            <b>Type</b>: string(80)                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    description                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Survey Channel                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    How will the survey happen?                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Dedicated Channel                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    Deactivate previous waves using this channel                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    scheduleType                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Prompt Channel                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    How will the prompting happen?  Leave empty if same as survey                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
<<<<<<< HEAD
                    marking                </th>
                <td>
                                            <b>Type</b>: string(32)                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
=======
                    Source Channel                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    For Import or Interview                </td>
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
            </tr>
                    </tbody>
    </table>
    </div>


WebInterview Schedule
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `schedule Tab in the WebInterview Wave
<http://behattest.stagingsurvos.com/waves/dummy/WebInterview#schedule>`_.

.. figure::  /images/modules/ongoing_WebInterview_schedule.png

   Rendered Form WebInterview Wave Tab schedule

.. raw:: html

    <div class="wy-table-responsive">
    <table border="1" class="docutils">
        <colgroup>
        <col width="15%">
        <col width="25%">
        <col width="60%">
        </colgroup>
        <thead valign="bottom">
            <tr class="row-odd">
                <th class="head">Field</th>
                <th class="head">Info</th>
                <th class="head">Description</th>
            </tr>
        </thead>
        <tbody valign="top">
                                    <tr class="row-odd">
                <th class="head">
                    duration                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Number of days a participant is enrolled                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
<<<<<<< HEAD
                    OK to Enroll                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    If enrollment is permitted now                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
=======
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
                    Schedule                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    help_block_schedule_configuration                </td>
            </tr>
<<<<<<< HEAD
                                    <tr class="row-even">
=======
                                    <tr class="row-odd">
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
                <th class="head">
                    Scheduling Conditions                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Only schedule when these conditions are met, e.g. dayOfWeek in ['Mon','Wed','Fri'] and dayOfMonth != 22
                                Fields: dayOfWeek (.e.g Mon), month (e.g. Jan), dayOfMonth (e.g. 15)                </td>
            </tr>
<<<<<<< HEAD
                                    <tr class="row-odd">
=======
                                    <tr class="row-even">
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
                <th class="head">
                    Start Date                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    Starting date of the protocol, when surveys are scheduled / accepted.                </td>
            </tr>
<<<<<<< HEAD
=======
                                    <tr class="row-odd">
                <th class="head">
                    Completion Threshold                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Minimum completed prompt percentage to mark as Complete                </td>
            </tr>
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
                                    <tr class="row-even">
                <th class="head">
                    Relative To Start Date                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    +1 for starting the next day                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Specific Start Date                </th>
                <td>
                                            <b>Type</b>: datetime                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Only if type is set to specific, otherwise calculated                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
<<<<<<< HEAD
                    Completion Threshold                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Minimum completed prompt percentage to mark as Complete                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
=======
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
                    Notes                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
<<<<<<< HEAD
                                    <tr class="row-even">
=======
                                    <tr class="row-odd">
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
                <th class="head">
                    Is Active                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Uncheck to disable and archive                </td>
            </tr>
                    </tbody>
    </table>
    </div>


WebInterview Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `enrollment Tab in the WebInterview Wave
<http://behattest.stagingsurvos.com/waves/dummy/WebInterview#enrollment>`_.

.. figure::  /images/modules/ongoing_WebInterview_enrollment.png

   Rendered Form WebInterview Wave Tab enrollment

.. raw:: html

    <div class="wy-table-responsive">
    <table border="1" class="docutils">
        <colgroup>
        <col width="15%">
        <col width="25%">
        <col width="60%">
        </colgroup>
        <thead valign="bottom">
            <tr class="row-odd">
                <th class="head">Field</th>
                <th class="head">Info</th>
                <th class="head">Description</th>
            </tr>
        </thead>
        <tbody valign="top">
                                    <tr class="row-odd">
                <th class="head">
                    Auto-Schedule                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    When a member registers via text or the web, schedule their assignments immediately                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Auto-Enroll                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    When a member registers via text or the web, automatically enroll them in this wave                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Tracked                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Capture Location with Web Survey                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Protocol                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Auto Populate Data                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Automatically update  data   with results                </td>
            </tr>
                    </tbody>
    </table>
    </div>


WebInterview Expiration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `expiration Tab in the WebInterview Wave
<http://behattest.stagingsurvos.com/waves/dummy/WebInterview#expiration>`_.

.. figure::  /images/modules/ongoing_WebInterview_expiration.png

   Rendered Form WebInterview Wave Tab expiration

.. raw:: html

    <div class="wy-table-responsive">
    <table border="1" class="docutils">
        <colgroup>
        <col width="15%">
        <col width="25%">
        <col width="60%">
        </colgroup>
        <thead valign="bottom">
            <tr class="row-odd">
                <th class="head">Field</th>
                <th class="head">Info</th>
                <th class="head">Description</th>
            </tr>
        </thead>
        <tbody valign="top">
                                    <tr class="row-odd">
                <th class="head">
                    Minutes before expiration                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Number of Reminders before Expiration                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    If 0, no reminders                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Maximum response time                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Time since first response (in minutes) before marking as Abandoned                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Number of warnings                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Once responding, number of warnings before marking as Abandoned                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Minimum Time Between Same Surveys                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Delay surveys if necessary by this amount (in minutes)                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
<<<<<<< HEAD
                    Reminder Message                </th>
=======
                    End Message                </th>
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
<<<<<<< HEAD
                    Warning Message                </th>
=======
                    Reminder Message                </th>
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
<<<<<<< HEAD
                    </tbody>
    </table>
    </div>


WebInterview Messages
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `messages Tab in the WebInterview Wave
<http://behattest.stagingsurvos.com/waves/dummy/WebInterview#messages>`_.

.. figure::  /images/modules/ongoing_WebInterview_messages.png

   Rendered Form WebInterview Wave Tab messages

.. raw:: html

    <div class="wy-table-responsive">
    <table border="1" class="docutils">
        <colgroup>
        <col width="15%">
        <col width="25%">
        <col width="60%">
        </colgroup>
        <thead valign="bottom">
            <tr class="row-odd">
                <th class="head">Field</th>
                <th class="head">Info</th>
                <th class="head">Description</th>
            </tr>
        </thead>
        <tbody valign="top">
                                    <tr class="row-odd">
                <th class="head">
                    welcomeMessage                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Message text                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    welcomeMessage                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    welcomeMessage Message                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    taskEndMessage                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Message text                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    taskEndMessage                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    taskEndMessage Message                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    endMessage                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Message text                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    endMessage                </th>
=======
                                    <tr class="row-even">
                <th class="head">
                    Expiration Message                </th>
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
<<<<<<< HEAD
                    endMessage Message                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    expirationMessage                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Message text                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    expirationMessage                </th>
=======
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Warning Message                </th>
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
<<<<<<< HEAD
                    expirationMessage Message                </td>
=======
                                    </td>
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d
            </tr>
                    </tbody>
    </table>
    </div>


WebInterview Extra
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `additional Tab in the WebInterview Wave
<http://behattest.stagingsurvos.com/waves/dummy/WebInterview#additional>`_.

.. figure::  /images/modules/ongoing_WebInterview_additional.png

   Rendered Form WebInterview Wave Tab additional

.. raw:: html

    <div class="wy-table-responsive">
    <table border="1" class="docutils">
        <colgroup>
        <col width="15%">
        <col width="25%">
        <col width="60%">
        </colgroup>
        <thead valign="bottom">
            <tr class="row-odd">
                <th class="head">Field</th>
                <th class="head">Info</th>
                <th class="head">Description</th>
            </tr>
        </thead>
        <tbody valign="top">
                    </tbody>
    </table>
    </div>


