Exercise Monitoring
=======================================
Suppose you wanted to know how much people excercised?  You could ask them to keep a diary, but people often forget to fill it out.  In this tutorial, we'll set up a nightly text message to ask people a few simple questions about their exercise for the day.  

 .. figure:: http://dummyimage.com/300x800/000/fff&text=sms+transcript
   :width: 300 px
   :alt: SMS Transcript of Exercise Survey
   :align: left

This tutorial shows how to set up a regularly scheduled survey, like a daily diary.

Design the Survey
------------------
NOTE: Although there's not much typing in this survey, if you want to simply import the survey and skip the typing, read "Importing Surveys" and import the survey called "Exercise 1".

Click on the Surveys menu, and then *Create a New Survey*.  You'll be prompted for the code, and the deployment methods.  You can deploy the same survey via multiple methods, selecting *how* you will deploy it now will make sure that the survey designer only allows you to create valid questions for your deployment type.  For example, you can't create a *camera* question via IVR.

Make the survey code exercise1, set the "Deployable via" to "SMS" and click on "Continue".  Survey Designer will open.  

The first question should be filled out like the image below.

 .. figure:: http://dummyimage.com/600x400/000/fff&text=survey+designer
   :width: 600 px
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

4. Publish the surveys

Exporting Collected Data
++++++++++++++++++++++

Go to Export

