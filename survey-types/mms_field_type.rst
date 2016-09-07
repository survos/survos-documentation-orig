.. This file was automatically generated from SCRIPT_NAME -- do not modify it except to change the relevant twig file!

..  _mms_field_type:

mms_field: Field Surveys via Text Message with Photos Survey
=======================================


Basic Workflow
-------------------------
* Configure a Field Surveys via Text Message with Photos Survey
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

Go through each screen of the Wave Form or Wizard for a mms_field Wave

Basic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


These are the fields in tab basic.   This is what it should look like: Taburl_.

.. _Taburl: http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=mms_field#basic


.. image::  http://dummyimage.com/600x400/000/fff&text=mms_field+Wave+Tab+basic
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form mms_field Wave Tab basic

This image will be generated from http://field.l.stagingsurvos.com/wave_repo/new?surveyType=mms_field#basic

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
                    Field Workers                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Separated By commas, empty means everyone is eligible                </td>
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


Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


These are the fields in tab enrollment.   This is what it should look like: Taburl_.

.. _Taburl: http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=mms_field#enrollment


.. image::  http://dummyimage.com/600x400/000/fff&text=mms_field+Wave+Tab+enrollment
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form mms_field Wave Tab enrollment

This image will be generated from http://field.l.stagingsurvos.com/wave_repo/new?surveyType=mms_field#enrollment

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
                                                <b>Validation</b>: Not blank, Min length: 2, Max length: 20<br>                                    </td>
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

.. _Taburl: http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=mms_field#workflow


.. image::  http://dummyimage.com/600x400/000/fff&text=mms_field+Wave+Tab+workflow
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form mms_field Wave Tab workflow

This image will be generated from http://field.l.stagingsurvos.com/wave_repo/new?surveyType=mms_field#workflow

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


Routing
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


These are the fields in tab routing.   This is what it should look like: Taburl_.

.. _Taburl: http://survos.l.stagingsurvos.com/wave_repo/new?surveyType=mms_field#routing


.. image::  http://dummyimage.com/600x400/000/fff&text=mms_field+Wave+Tab+routing
    :height: 400
    :width: 600
    :scale: 50
    :alt: Rendered Form mms_field Wave Tab routing

This image will be generated from http://field.l.stagingsurvos.com/wave_repo/new?surveyType=mms_field#routing

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
                    MobilityPreference                </th>
                <td>
                                            <b>Type</b>: string(12)                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Cents/mile                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Minutes/Task                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    RouteDistance                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    RouteTime                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    include_route_points                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                    </tbody>
    </table>
    </div>



