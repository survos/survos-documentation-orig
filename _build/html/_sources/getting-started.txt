System Overview
======================

Survos is a set of components that allow researchers to collect data about study participants and/or data about "things", such as places or photos.

Each major system component, called a "module" can be run individually, they can also be combined.

Terminology
-----------
Here are some terms that are important to know.

- **Project** :  The data, people and protocols of a research study.

- **Module**: A collection of survey types that collect data in a similar way.  Because the types of data the system can collect is so varied, selectively installing modules allows the system to be
navigated more easily.  Many projects only use one or two modules.
 - *Import*: Import data from external source (e.g. csv file, CartoDB)
- **Survey Type**: A generic term describing a component of the Survos Platform that collects data.  If that data is personal (e.g. about a study participants), this is sometimes called an "intervention".  If it's about a place, it can be called a "field survey".  It can also be called a "Turk Job" if the data is being collected through Amazon's Mechanical Turk".
- **Survey Instrument** : a list of questions and answer options, tied to a how those questions will be deployed, such as via SMS or Turk or a Web Interview
- **Wave** : Deployment of the survey questions.  It is the central object in the system, and is the configuration for who will answer the survey questions, when, how, how often, how much they'll be paid, etc.  There are many types of jobs, and each type will have its own specific configuration, which will be described later in the document.
- **User (formerly Member)**: Accounts associated with a project.  All users have an identifier that is unique with in the project, for study participants, this is sometimes referred to as a "Subject ID", and except when testing, this identifier should not be personally identifiable.  There are various roles users have, such as "applicant", "participant", "turker" "researcher" and "participant".
- **Assignment/Survey Response**: The participant's survey answers.
- **Data**: Each project may contain its own database of places, images and other data.  Jobs that use data (e.g. visiting a list of places, looking at a list of photos) get their data from these tables.  Wave collect data (e.g. taking pictures) put their results here (so the results can be used by subsequent Surveys).

Data Collection Workflow
-------------------------

All data collection within a project works roughly the same way, and will be described in specific detail in each module.

# Within a module, decide *how* your questions will be delivered (e.g. SMS, Interview, Turk), and create a survey.
# Design your questions within the survey, paying special attention to the question codes, types and possible responses.  The data collected will be available using these codes.
# Define the specifics of your survey deployment, called a _wave_ -- this will change for each specific survey type, but is basically *who* receives the survey, *when* and how often.
* Deploy the wave and collect the data.  Wave Configuration is specific to each survey type, and is described in detail under "Deployment" for each Survey Type


Getting Started
-------------------

If your projects has study participants, enable one or more of these modules:

 - *:ref:`ongoing`*: Continously collection of data about a *participant*, .e.g an SMS survey 3x/day for 2 weeks, see :ref:`ongoing`
 - *Single*: A one-time questionnaire of a participant, e.g. "How often did your parents smoke indoors?"
 - *Tracking*: Continuous location data (works with tracking app that runs on participant's phone)

If your project needs anonymous, remote participants to answer questions about themselves, enable

 - *:ref:`opinion`*: Questions are answered by anonymous Turkers

If your project has or collects data about things, such as places or images, enable

 - *Turk Expert*: Questions are answered by a single, anonymous Turker about Object Data
 - *Turk Consensus*: Questions are answered by multiple, anonymous Turkers about Object Data

If your project has a list of places that need to be visited by field workers, install

 - *Field*: Questions about a list of places visited by field workers.

If your project needs to pre-qualify participants, field-workers, or turkers, install

 - *Screener*: Scored Surveys that pre-qualify participants or Turkers before they begin work.  Unpaid.

Because the modules can be run independently and that often a study needs only one or two modules, this documentation describes each module as if it were a separate project.  While a real-world study may enable multiple modules, keeping them separate makes it easier to learn and understand the system.  In the appendix there are examples of more complex configurations.

.. toctree::
   :maxdepth: 5

       modules/repetitive
       modules/single
       modules/opinion


