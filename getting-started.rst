Terminology
-----------
Here are some terms that are common to the Survos Platform.

Project
    The data, people and protocols of a research study.
Module
     A collection of survey types that collect data in a similar way.  Because the types of data the system can collect is so varied, selectively installing modules allows the system to be navigated more easily.  Many projects only use one or two `ref:modules.
Survey Type
    A generic term describing a component of the Survos Platform that collects data.  If that data is personal (e.g. about a study participants), this is sometimes called an "intervention".  If it's about a place, it can be called a "field survey".  It can also be called a "Turk Job" if the data is being collected through Amazon's Mechanical Turk".
Survey
    A list of questions and answer options, tied to a how those questions will be deployed, such as via SMS or Turk or a Web Interview
Wave
    Deployment of the survey questions.  It is the central object in the system, and is the configuration for who will answer the survey questions, when, how, how often, how much they'll be paid, etc.  There are many types of jobs, and each type will have its own specific configuration, which will be described later in the document.
Turk
    Amazon Mechanical Turk (AMT) is a marketplace for crowd-sourced work. The Posse Platform enables a user to create what AMT calls external HITs, which are tasks run outside of the AMT system. Internal hits for AMT are somewhat limited. With a Turk job, a task is posted and a crowd of anonymous users has a chance to accept individual assignments and complete the task. This is particularly good for gathering data about a photo, where if a group of anonymous people reach consensus about something, it is likely to be valid.


- **User (formerly Member)**: Accounts associated with a project.  All users have an identifier that is unique with in the project, for study participants, this is sometimes referred to as a "Subject ID", and except when testing, this identifier should not be personally identifiable.  There are various roles users have, such as "applicant", "participant", "turker" "researcher" and "participant".
- **Assignment/Survey Response**: The participant's survey answers.
- **Data**: Each project may contain its own database of places, images and other data.  Jobs that use data (e.g. visiting a list of places, looking at a list of photos) get their data from these tables.  Wave collect data (e.g. taking pictures) put their results here (so the results can be used by subsequent Surveys).
- *Import*: Import data from external source (e.g. csv file, CartoDB)

Data Collection Workflow
-------------------------

All data collection within a project works roughly the same way, and will be described in specific detail in each module.

#. Within a module, decide *how* your questions will be delivered (e.g. SMS, Interview, Turk), and create a survey.
#. Design your questions within the survey, paying special attention to the question codes, types and possible responses.  The data collected will be available using these codes.
#. Define the specifics of your survey deployment, called a _wave_ -- this will change for each specific survey type, but is basically *who* receives the survey, *when* and how often.
#. Deploy the wave and collect the data.  Wave Configuration is specific to each survey type, and is described in detail under "Deployment" for each Survey Type


