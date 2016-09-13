.. This file was automatically generated from SCRIPT_NAME -- do not modify it except to change the relevant twig file!

..  _sms_self_report_type:

SMS Self Report Surveys
=======================================
Self-Initiated SMS message

Basic Workflow
-------------------------
* Configure a SMS Self Report Survey
* Design Survey Questions
* Preview with Dummy Data
* Activate
* Recruit
* Collect

Typical Deployment Configuration
--------------------------------

* 3x/day for 14 days, randomly between participant wake time...

sms_self_report Wave Configuration
------------------------

Go through each screen of the Wave Form or Wizard for a sms_self_report Wave

sms_self_report Basic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `basic Tab in the sms_self_report Wave
<http://behattest.stagingsurvos.com/waves/dummy/sms_self_report#basic>`_.

.. figure::  https://s3.amazonaws.com/survos-documentation/sms_self_report_basic.png

   Rendered Form sms_self_report Wave Tab basic

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
                    Bulk Import                </th>
                <td>
                                            <b>Type</b>: string(24)                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    duration                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Number of days a participant is enrolled                </td>
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


sms_self_report Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `enrollment Tab in the sms_self_report Wave
<http://behattest.stagingsurvos.com/waves/dummy/sms_self_report#enrollment>`_.

.. figure::  https://s3.amazonaws.com/survos-documentation/sms_self_report_enrollment.png

   Rendered Form sms_self_report Wave Tab enrollment

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
                    Auto-Enroll                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    When a member registers via text or the web, automatically enroll them in this wave                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Notification                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Notify Designated Administrators with Survey Results                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Welcome                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Send a welcome text message upon enrollment                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Message                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Welcome Message                </td>
            </tr>
                    </tbody>
    </table>
    </div>


sms_self_report Workflow
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `workflow Tab in the sms_self_report Wave
<http://behattest.stagingsurvos.com/waves/dummy/sms_self_report#workflow>`_.

.. figure::  https://s3.amazonaws.com/survos-documentation/sms_self_report_workflow.png

   Rendered Form sms_self_report Wave Tab workflow

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
                    Incoming Queue                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    Incoming queue, for creating or updating assignments.  (need background task?)                </td>
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


sms_self_report Expiration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `expiration Tab in the sms_self_report Wave
<http://behattest.stagingsurvos.com/waves/dummy/sms_self_report#expiration>`_.

.. figure::  https://s3.amazonaws.com/survos-documentation/sms_self_report_expiration.png

   Rendered Form sms_self_report Wave Tab expiration

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
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Minutes since initial prompt before expiring                </td>
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
                    Maximum survey length                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Time since first response (in minutes) before marking as Abandoned                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Warning Frequency                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Once responding, minutes between warnings                </td>
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
                    End Message                </th>
                <td>
                                            <b>Type</b>: string(150)                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Reminder Message                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Expiration Message                </th>
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


sms_self_report Extra
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `additional Tab in the sms_self_report Wave
<http://behattest.stagingsurvos.com/waves/dummy/sms_self_report#additional>`_.

.. figure::  https://s3.amazonaws.com/survos-documentation/sms_self_report_additional.png

   Rendered Form sms_self_report Wave Tab additional

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
                    Disable Auto-enroll                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    Disable autoenroll for previous waves                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Purge Schedule                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    Purge all scheduled surveys for other waves in this survey                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    De-activate Waves                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    De-active previous waves in this survey                </td>
            </tr>
                    </tbody>
    </table>
    </div>


