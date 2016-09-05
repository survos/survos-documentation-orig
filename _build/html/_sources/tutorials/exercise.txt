Exercise Monitoring
=======================================
Suppose you wanted to know how much people excercised?  You could ask them to keep a diary, but people often forget to fill it out.  In this tutorial, we'll set up a nightly text message to ask people a few simple questions about their exercise for the day.  

 .. figure:: img-exercise/1-sms-transcript.png
   :width: 500 px
   :alt: SMS Transcript of Exercise Survey
   :align: left


This tutorial shows how a monitoring project is set up, and how the monitoring features work on the FLOW dashboard and the FLOW app. We start by introducting a real-life example.

.. container:: clearer

    .. image:: /img/spacer.png

Design the Survey
------------------
NOTE: Although there's not much typing in this survey, if you want to simply import the survey and skip the typing, read "Importing Surveys" and import the survey called "Exercise 1".

Click on the Surveys menu, and then *Create a New Survey*.  You'll be prompted for the code, and the deployment methods.  You can deploy the same survey via multiple methods, selecting *how* you will deploy it now will make sure that the survey designer only allows you to create valid questions for your deployment type.  For example, you can't create a *camera* question via IVR.

Make the survey code exercise1, set the "Deployable via" to "SMS" and click on "Continue".  Survey Designer will open.  

The first question should be filled out like the image below.

 .. figure:: img-exercise/2-designer.png
   :width: 500 px
   :alt: First Question of Exercise Survey
   :align: left

Adding Questions
++++++++++++++++++++++++++++++
To add the first question to a survey, follow these steps:

1. Fill out the question text with **Did you exercise today?**  This is a Yes/No question, so choose that as the type from the dropdown menu. Each question has its own code, like the column headers in a spreadsheet or analysis in a statistics program like R or Stata.  Type "exercised_today" as the variable.

 We could stop here, if that's all the data we wanted to collect.  But let's say we're interested in what kind of exercise, so let's ask.

2. Add another question by clicking on the ADD QUESTION button. Now fill out the second question with **"What kind of exercise?"**, and make the variable name "exercise_type".  We could let the user answer whatever they wanted, but this would give us all sorts of variations that would be difficult to analyse.  So we'll restrict the answers by making it a radio question, called that way because like a radio, you can only choose one station at a time.  Choose "radio" from the dropdown, and in the Choices, create answers like these:

IMAGE: 1 Running, 2 Team Sports 3: Swimming 4: Yoga 5:Other

We could stop here, but let's say we're interested in the relationship between exercise and feeling, so let's ask. 

3. Add another question by clicking on the ADD QUESTION button, and enter "On a scale of 1-5, where 1 is lousy and 5 is great, how do you feel right now?".  Set the type to integer, and to make sure the answers are in the appropriate range, set min to 1 and max to 5.

IMAGE OF QUESTION.

Let's do a quick look 

2. Click the blue 'Make monitoring group' button on the top. After accepting the popup notification, this will change to 'Monitoring Enabled', and show a dropdown where you can select one of the surveys in this group as the survey that creates new Wemonitored entities. As we don't have any surveys yet, this dropdown is still empty.

3. Create the surveys you need, just as you would create normal surveys. In the survey that will be used to create new records, there are two checkboxes which are important. 
   a. The first one is *Use in record display*, which is shown on free text questions. When this is checked, the answer to this question will become part of the 'name' of the record. This will be shown in lists on the device, and can be used to search records. By default, this is off. This should only be enabled for one or two questions which will help to identify the record, such as an id, or a name. Multiple values will be added together separated by a dash '-'.
   b. The second one is *Use as record location*, which is shown on geolocation questions. When this is checked, the location captured by this question will be used as the main location of the record. By default, this is turned on.

 .. figure:: img-monitoring/2-monitoring.png
   :width: 500 px
   :alt: Illustration of monitoring
   :align: left

4. Publish the surveys

5. After the surveys are created, select one of them using the dropdown box in the survey group overview. This survey gets the special role of 'registration survey', and is capable of creating new records on the device.

.. container:: clearer

    .. image:: /img/spacer.png

Structuring your survey forms
++++++++++++++++++++++++++++++
Because you can use different forms to collect data on a record, the question comes up what questions to ask in which forms. The guideline to follow is this:

* Information captured once - Information that identifies the entity you are monitoring should go in the survey that creates the record. For example, if you monitor a water meter, you would create a 'water meter registration' form, which captures the name of the owner, his/her address, and the meter id. Not more.

* Information tracked over time — Information about the entity that will probably change, and that you want to track over time, should go in a different form. For example, you might have a 'water meter reading' form, which just captures the current water meter reading and a photo of the water meter. Or, if you are monitoring patients in a hospital, you could have 'blood test', and 'psychological test' forms. 

Viewing record data
++++++++++++++++++++
To see which records are available for a monitoring project, open the 'Monitoring' subtab on the 'Data' tab. There, you can select the survey group that contains the monitoring project, and you will see a table with the records within that project. The table shows 'identifier', 'display name', and 'last update'. The identifier is the unique identifier of the record. The display name is derived from answers to questions in the 'registration' form. The setting 'display in record list on device' on free text questions determines if answers to that question become part of the display name.

 .. figure:: img-monitoring/3-monitoring.png
   :width: 800 px
   :alt: Illustration of monitoring
   :align: center

When you click 'view details' on any one of the records in the table, you will see the survey responses that are part of a single record. For each submitted survey response, the survey, submitter, device, and collection data are displayed.

When you click 'view details' on a survey response, you will see the individual answers given to the questions in that response.

Exporting record data
++++++++++++++++++++++
To export data, go to the 'Reports' tab, and select the 'Export reports' subtab. Here, you can select a survey group and survey form, and . If you select a survey group that is also a monitored group, a checkbox 'Export only last collection' will be displayed. When this is enabled, only the latest collected data for that survey will be exported. For example, if you have collected water several meter readings for a single water meter, and this checkbox is selected, only the last one will be exported. 

 .. figure:: img-monitoring/4-monitoring.png
   :width: 800 px
   :alt: Illustration of monitoring
   :align: center

The exported file will contain the record identifier and the display name as the first two columns. 

In a real-life situation, you might want to export a report which combines answers from different forms. For example, if you are monotoring water meters, you might want to export a file which has the customer name and address, plus the latest value of the water meter reading. At the moment, this type of exporting is not yet possible, but it will be made available in a future version of FLOW.

In the mean time, you can use an excel technique to match data accross different files, based on the identifier of each record. This uses the VLOOKUP function, as described `in this article <http://howtovlookupinexcel.com/vlookup-between-two-workbooks>`_  and `this instruction movie <https://www.youtube.com/watch?v=809m6kLTfgI>`_. If you need help in implementing this, please contact us as support@akvoflow.org


Monitoring - FLOW app
----------------------
 .. figure:: img-monitoring/5-monitoring.png
   :width: 200 px
   :alt: Illustration of monitoring
   :align: left

When the app is opened for the first time, it will sync with the server and display the survey groups that contain surveys that have been assigned to the device. Normal survey groups just contain surveys, which can be used to collect data as usual. A survey group which is also a monitoring group is different: it contains both the records for a monitored entitiy, and the survey forms which are used to create new forms or add additional information to them.



.. container:: clearer

    .. image:: /img/spacer.png

Syncing records
++++++++++++++++++++++
To sync records, first make sure that you have a good wifi or 3G connectivity. Downloading a large number of records can involve quite some data, which is why it is important to have a good connection. If you sure the connection is ok, follow these steps:

1. Select the monitoring group that you want to work with.

2. Click on the 'more' button in the top right (three vertical dots), and select 'Sync records'

3. The records will be synced, and a message in the notification bar will show the progress and how many records have been synced.

 .. figure:: img-monitoring/6-monitoring.png
   :width: 1000 px
   :alt: Illustration of monitoring
   :align: center

The syncing process is optimised to only download the latest information — any records that have not changed since the last download will not be downloaded again.

Syncing records is not an automatic process, so it needs to be manually performed whenever the enumerator needs the latest updates from the server.

Creating a new record
++++++++++++++++++++++
A new record can be created by clicking the '+' icon, which is shown on the top of the list of records. When a new record is first created, only the special 'registration' form can be selected. This is needed to capture the identifying information for the new record. When this first form has been submitted, other forms become available.

 .. figure:: img-monitoring/7-monitoring.png
   :width: 1000 px
   :alt: Illustration of monitoring
   :align: center

Searching for an existing record
+++++++++++++++++++++++++++
To find a record, follow one of these steps:

1. By default, the list of records is sorted by distance, with the nearest record shown first. For this to work, the GPS of the device needs to be active. To select a record, click it. By clicking the 'more' icon (three vertical dots) and selecting 'order by', you can also order the records by date, with the most recently changed first.

2. By clicking the 'map' tab, a map is shown with all the records, centered on your present location. If you click a record marker it will show the display name and the identifier. If you click that text, the record will be selected.

3. If you click the 'search' icon and start typing, a list of filtered records will be shown. The text you type is compared to both the display text and the identifier. 

 .. figure:: img-monitoring/8-monitoring.png
   :width: 600 px
   :alt: Illustration of monitoring
   :align: center

Adding information to an existing record
+++++++++++++++++++++++++++++++++++++++++
When you have selected a record, the record display name and identifier are displayed, plus a list of available surveys. To add information to the selected record, select a survey, fill it, and submit it.

If the record already contains a previous filled-in version of that survey, the mobile device will prompt the user if he/she wants to prefill the new, empty survey with the previously collected values. If the users selects 'ok', a fresh copy of the survey is opened, with the previous values filled in. 

 .. figure:: img-monitoring/9-monitoring.png
   :width: 1000 px
   :alt: Illustration of monitoring
   :align: center

It is important to understand that the previous values will not be overwritten — only new information will be added. This is true in general: only new facts are created and stored, old values are never overwritten. This protects data against human error.

Updating information collected by the 'registration' form
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 .. figure:: img-monitoring/10-monitoring.png
   :width: 300 px
   :alt: Illustration of monitoring
   :align: left

Usually, the registration form is only used once, when the record is first created. That is why that survey is shown in a different (red) color.

However, sometimes data collected by this survey needs to be updated, for example in the case of a spelling mistake. That is why the survey can still be accessed. When the enumerator clicks this survey, a warning message is displayed. When the enumerator accepts this, they can prefill the survey with the existing values, and update them by making the required changes and submitting the survey.
