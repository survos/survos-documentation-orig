Survos Platform
===============

The Survos Platform provides researchers with powerful tools to interact with their study participants.  Participants can interact via random or fixed-interval SMS surveys, provide detailed, continuous information about their location, and collect photos via SMS or our app.  Researchers can extract information about those photos via Amazon's Mechanical Turk, a crowd-sourcing platform.

This documentation provides detailed instructions about what the tools do, and how they are configured.  As with many comprehensive systems, sometimes getting started is the hardest part.  The major parts of the data collection system are broken down into "Modules".  The basic workflow is the same for all the survey types.

Getting Started
---------------

If your projects has study participants, enable one or more of these modules:

 - *Ongoing*: Continous collection of data about a *participant*, .e.g an SMS survey 3x/day for 2 weeks, see :ref:`ongoing`
 - *Single*: A questionnaire of a participant, often web-based, e.g. "How often did your parents smoke indoors?" *disabled*
 - *Tracking*: Continuous location data (works with tracking app that runs on participant's phone) see *disabled*

We integration with Amazon's Mechanical Turk, to do the following:

 - *Turk Opinion*: Questions are answered by anonymous Turkers see *disabled*
 - *Turk Expert*: Questions are answered by a single, anonymous Turker about an image, place or other piece of data
 - *Turk Consensus*: Questions about things (not people) are answered by multiple, anonymous Turkers until consensus is reached.

If your project has a list of places that need to be visited by field workers, install

 - *Field*: Questions about a list of places visited by field workers.

If your project needs to pre-qualify participants, field-workers, or turkers, install

 - *Screener*: Scored Surveys that pre-qualify participants or Turkers before they begin work.  Unpaid.

Because the modules can be run independently and that often a study needs only one or two modules, this documentation describes each module as if it were a separate project.  While a real-world study may enable multiple modules, keeping them separate makes it easier to learn and understand the system.  In the appendix there are examples of more complex configurations.


Contents:

.. toctree::
    :maxdepth: 1

    getting-started
    workflows
    roles
    modules
    integration-types
    users-participants
    tutorials
    tracking






Indexes and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
