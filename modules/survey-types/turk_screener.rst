.. This file was automatically generated from SCRIPT_NAME -- do not modify it except to change the relevant twig file!

..  _turk_screener_type:

Turk Qualifications Surveys
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

turk_screener Wave Configuration
------------------------

Go through each screen of the Wave Form or Wizard for a turk_screener Wave

turk_screener Basic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `basic Tab in the turk_screener Wave
<http://behattest.stagingsurvos.com/waves/dummy/turk_screener#basic>`_.

.. image::  https://s3.amazonaws.com/survos-documentation/turk_screener_basic.png
    :alt: Rendered Form turk_screener Wave Tab basic

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


turk_screener Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `enrollment Tab in the turk_screener Wave
<http://behattest.stagingsurvos.com/waves/dummy/turk_screener#enrollment>`_.

.. image::  https://s3.amazonaws.com/survos-documentation/turk_screener_enrollment.png
    :alt: Rendered Form turk_screener Wave Tab enrollment

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


turk_screener Workflow
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `workflow Tab in the turk_screener Wave
<http://behattest.stagingsurvos.com/waves/dummy/turk_screener#workflow>`_.

.. image::  https://s3.amazonaws.com/survos-documentation/turk_screener_workflow.png
    :alt: Rendered Form turk_screener Wave Tab workflow

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
                    Goal                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Goal for the number of participants for this wave                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Max                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Maximum number of participants for this wave                </td>
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
                    Auto Populate Data                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Automatically update member data   with results                </td>
            </tr>
                    </tbody>
    </table>
    </div>


turk_screener Qualifications
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `qualifications Tab in the turk_screener Wave
<http://behattest.stagingsurvos.com/waves/dummy/turk_screener#qualifications>`_.

.. image::  https://s3.amazonaws.com/survos-documentation/turk_screener_qualifications.png
    :alt: Rendered Form turk_screener Wave Tab qualifications

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
                    Title                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Seen by Turkers                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Description                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Seen by Turkers                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Qualification Code                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    will be prefixed by project code, then used in Qualification Type Text                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Test Duration                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Time to complete (in seconds)                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Retry Delay                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    Time before they can take qualification again (in seconds)                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Keywords                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    QT Keywords cannot be modified after publishing                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Post-Processing                </th>
                <td>
                                            <b>Type</b>: string(64)                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Post-processing Method, system administrators only                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Automatically Grant -- NO TEST                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Auto Grant Value                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    value to assign if automatically granted/approved and not isScored                </td>
            </tr>
                    </tbody>
    </table>
    </div>


