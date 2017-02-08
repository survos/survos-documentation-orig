.. This file was automatically generated from SCRIPT_NAME -- do not modify it except to change the relevant twig file!

..  _Simulator_integration_type:

Simulator Integration Types
=======================================
Simulator

The purpose of this integration is to provide a channel to collect data.


Simulator Wave Configuration
------------------------

Go through each screen of the Wave Form or Wizard for a Simulator Wave

Simulator Basic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `basic Tab in the Simulator Wave
<http://behattest.stagingsurvos.com/waves/dummy/Simulator#basic>`_.

.. figure::  /images/modules/ongoing_Simulator_basic.png

   Rendered Form Simulator Wave Tab basic

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
                    marking                </th>
                <td>
                                            <b>Type</b>: string(32)                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                    </tbody>
    </table>
    </div>


Simulator Schedule
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `schedule Tab in the Simulator Wave
<http://behattest.stagingsurvos.com/waves/dummy/Simulator#schedule>`_.

.. figure::  /images/modules/ongoing_Simulator_schedule.png

   Rendered Form Simulator Wave Tab schedule

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
                    Schedule                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    help_block_schedule_configuration                </td>
            </tr>
                                    <tr class="row-even">
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
                                    <tr class="row-odd">
                <th class="head">
                    Start Date                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    Starting date of the protocol, when surveys are scheduled / accepted.                </td>
            </tr>
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
                    Notes                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
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


Simulator Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `enrollment Tab in the Simulator Wave
<http://behattest.stagingsurvos.com/waves/dummy/Simulator#enrollment>`_.

.. figure::  /images/modules/ongoing_Simulator_enrollment.png

   Rendered Form Simulator Wave Tab enrollment

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


Simulator Expiration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `expiration Tab in the Simulator Wave
<http://behattest.stagingsurvos.com/waves/dummy/Simulator#expiration>`_.

.. figure::  /images/modules/ongoing_Simulator_expiration.png

   Rendered Form Simulator Wave Tab expiration

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
                    Reminder Message                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Warning Message                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                    </tbody>
    </table>
    </div>


Simulator Messages
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `messages Tab in the Simulator Wave
<http://behattest.stagingsurvos.com/waves/dummy/Simulator#messages>`_.

.. figure::  /images/modules/ongoing_Simulator_messages.png

   Rendered Form Simulator Wave Tab messages

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
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
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
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    expirationMessage Message                </td>
            </tr>
                    </tbody>
    </table>
    </div>


Simulator Extra
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `additional Tab in the Simulator Wave
<http://behattest.stagingsurvos.com/waves/dummy/Simulator#additional>`_.

.. figure::  /images/modules/ongoing_Simulator_additional.png

   Rendered Form Simulator Wave Tab additional

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


