.. This file was automatically generated from SCRIPT_NAME -- do not modify it except to change the relevant twig file!

..  _turk_opinion_type:

turk_opinion: Turk Opinion Survey
=======================================


Basic Workflow
-------------------------
* Configure a Turk Opinion Survey
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

Go through each screen of the Wave Form or Wizard for a turk_opinion Wave

Basic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


These are the fields in tab basic.   This is what it should look like: Taburl_.

.. _Taburl: http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=turk_opinion#basic


.. image::  http://dummyimage.com/600x400/000/fff&text=turk_opinion+Wave+Tab+basic
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form turk_opinion Wave Tab basic

This image will be generated from http://opinion.l.stagingsurvos.com/wave_repo/new?surveyType=turk_opinion#basic

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
                    Notes                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
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


Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


These are the fields in tab enrollment.   This is what it should look like: Taburl_.

.. _Taburl: http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=turk_opinion#enrollment


.. image::  http://dummyimage.com/600x400/000/fff&text=turk_opinion+Wave+Tab+enrollment
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form turk_opinion Wave Tab enrollment

This image will be generated from http://opinion.l.stagingsurvos.com/wave_repo/new?surveyType=turk_opinion#enrollment

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
                    </tbody>
    </table>
    </div>


Workflow
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


These are the fields in tab workflow.   This is what it should look like: Taburl_.

.. _Taburl: http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=turk_opinion#workflow


.. image::  http://dummyimage.com/600x400/000/fff&text=turk_opinion+Wave+Tab+workflow
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form turk_opinion Wave Tab workflow

This image will be generated from http://opinion.l.stagingsurvos.com/wave_repo/new?surveyType=turk_opinion#workflow

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
                    Turk Deployment                </th>
                <td>
                                            <b>Type</b>: string(12)                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                                    </td>
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
                    Auto Publish                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Auto-publish tasks to Turk/Import when queued                </td>
            </tr>
                    </tbody>
    </table>
    </div>


Task
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


These are the fields in tab task.   This is what it should look like: Taburl_.

.. _Taburl: http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=turk_opinion#task


.. image::  http://dummyimage.com/600x400/000/fff&text=turk_opinion+Wave+Tab+task
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form turk_opinion Wave Tab task

This image will be generated from http://opinion.l.stagingsurvos.com/wave_repo/new?surveyType=turk_opinion#task

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
                    Task Title                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Seen by Workers                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Description                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Seen by Workers                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Deployment Keywords                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Keywords make searching for jobs easier                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Reward                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    in USD, can be formula                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Repetitions                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Number of Repetitions (aka raters)                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    HIT Lifeftime                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    e.g. 1d 3h 5m for 1 day, 3 hour and 5 minutes                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Time Worker has to complete assignment                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Auto Approval                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Amount of time before Assignment is automatically approved "
                            ."(faster if consensus reached)                </td>
            </tr>
                    </tbody>
    </table>
    </div>


Qualifications
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


These are the fields in tab qualifications.   This is what it should look like: Taburl_.

.. _Taburl: http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=turk_opinion#qualifications


.. image::  http://dummyimage.com/600x400/000/fff&text=turk_opinion+Wave+Tab+qualifications
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form turk_opinion Wave Tab qualifications

This image will be generated from http://opinion.l.stagingsurvos.com/wave_repo/new?surveyType=turk_opinion#qualifications

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
                    Use Qualifications                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Restrict tasks to qualified people                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Locale                </th>
                <td>
                                            <b>Type</b>: string(32)                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    MinApprovalRate                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    MinApprovedHits                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Qualifications                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    SET THESE IN JOB! <strong>Valid qualification types are: </strong> . <br><strong>Valid operators are: </strong>                 </td>
            </tr>
                    </tbody>
    </table>
    </div>


