Tracking
========

The Posse Platform allows the ability to track people's location by associating a tracking ID with each participant.
Tracks (timestamped coordinates) are sent to an independent tracking server, Survos Tracker. Individual projects
pull tracking data from the participants locally, as needed.

This section will review various methods to initiate tracking, and how to integrate tracking with the Posse Platform.

GT500 Devices
-------------

The GT500 devices are programmed either with the Queclink software and USB cable provided to device administrators
or remotely via SMS. The device should be programmed to send the data to the same address as Traccar—that is:

==============  ==================
Setting         Value
==============  ==================
Server address  tracker.survos.com
Server port     5000
==============  ==================

The unique identifier for GT500 devices is always the IMEI number, a string of 15 digits unique to each device.
A name can also be programmed, such as *SCTC-105*, but this is simply a tool to make debugging a bit easier.

Survos Mobile
-------------

Survos Mobile has built-in tracking and currently does not have any configuration options.

Traccar
-------

Traccar is a free and open source GPS tracking system. Tracking apps are available for Android and iOS
that integrate with the Traccar server or any server that can understand their protocol. Since the Survos Tracker
server understands that protocol, a user simply needs to download the app and configure it to point to the right server.

Since the software is available in the app stores, installation is very easy:

* Android: https://play.google.com/store/apps/details?id=org.traccar.client for remote install.
* Android or iOS: Open the App Store on your device, search for *Traccar Client* and install.

Traccar Configuration
^^^^^^^^^^^^^^^^^^^^^

Once you've opened the application, Simply tap on each setting to be prompted for the new value. Use these
values to point your device to Survos Tracker. The initial version of Traccar for iOS does not include
Location Provider or Extended Format, although the author has indicated that these may be added in the future.

.. figure:: images/traccar-android.jpg
   :width: 300px
   :alt: Traccar Configuration for Android
   :name: Traccar Configuration for Android
   :height: 450px
.. figure:: images/traccar-iphone.png
   :width: 300px
   :height: 450px
   :alt: Traccar Configuration for Iphone
   :name: Traccar Configuration for Iphone


=================  ===================================================================================================
Setting            Value
================= ====================================================================================================
Device identifier  Any unique string, such as participant email or the internal device identifier that it defaults to.
Server address     tracker.survos.com
Server port        5000
Frequency          60 (or set according to your project requirements)
Location Provider  Android Only: Mixed
Extended Format    Android Only: Checked
Service status     Turn on when everything is configured
=================  ===================================================================================================

Please note that Apple now prevents apps that use the location service from automatically starting when the phone is
powered on. Therefore participants are responsible for turning the app when they boot their phone up, or (even better)
keeping their phone charged so it never goes off.  Because location apps are a battery drain, this is often difficult.
You can use the Posse Platform to schedule nightly "surveys" that remind people to plug their devices in and ask them
to report any problems.

Integration with the Posse Platform
-----------------------------------

Survos Tracker simply records a timestamp and point (latitude and longitude) for each device that sends it
information. In order to integrate it with the Posse Platform, there must be a link between users and the device.
This can be done either by the user, if they are managing their own account, or by a project administrator, if it
is a closed project.

A closed project can only be managed by someone with an account set up that allows access to user data on the
system. This is usually the administrator's account.

See :doc:`users-participants/enrolling-participants`.

Registering Devices
^^^^^^^^^^^^^^^^^^^

In order to associate a tracking device with a user, use the Device panel at the bottom of the profile screen.
The GT500's  must be registered with the Master Device Database before those devices can be
added to a user profile. The GT500's are registered at the American Legacy Foundation before they are shipped
to partners.  Traccar devices will register themselves the first time a point is received by the Survos Tracking Server.

.. figure:: images/survos-profile-edit.png
   :width: 700

   Survos Device Editor

Closed Project Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^

Projects may be completely closed, (not allowing users to self-enroll or access their data), or they can
allow for some user participation. In particular, a project might allow a user to sign up online or in a
waiting area before their initial interview. This will allow the user to type in their own name and cell
phone number, and then the administrator can simply verify it and add the tracking device as necessary.

If the project is completely closed, then the administrator needs to create a user record for the participant.
To do that, simply click on the *Create a New User* link.

.. figure:: images/create-a-new-user.png
   :width: 700

   New User Administration

While this screen is fairly self-explanatory, there are a few things worth noting:

* **Username:** This is the identifier that will show up on reports and data exports. You can select something
  obscure if you want to keep your report data anonymous. You can also choose an email address, since that
  will be unique. Or depending on the project size, you may choose something like first initial plus last name.
  There should be no spaces or punctuation in the username (other than "@" and "." for email addresses).
  It is simply a code for the user.
* **Name:** Used in some reports, but mostly for administration.
* **Timezone:** Timezone is important with tracking and scheduled surveys, since surveys are often scheduled
  during waking hours, so the system needs to know the timezone. The default is the timezone where the
  computer is located, which may be wrong if the participant is being registered remotely, such as over the phone.
* **User Roles:** Gives special permissions to certain users, such as administrative rights.
* **Amazon Turk Id:** If you are paying participants through Amazon Mechanical Turk, this is their account
  number. User recruitment can also be done via Mechanical Turk, as described in the section "Creating a
  Recruitment Job" in the "Surveys" chapter.
* **Mobile Phone:** Required to participate in SMS (text) or MMS (text plus photos) mobile surveys. Note that
  Google Voice will not work with MMS, but does work with SMS surveys.
* **Tracking Device Id:** This is the IMEI (for GT500 devices) or other unique identifier that is being sent to Survos Tracker.

Conclusion
----------

User registration is fairly straightforward. It can be done entirely by an administrator, entirely
self-administered, or a combination. The user record is a single system-wide way to maintain important
information about a single user, such as the email address, timezone, mobile phone, and tracking device.

Once a user is set up in the system, they can participate in mobile surveys.  
