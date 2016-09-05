Users and Participants
======================

A *user* an individual who has an account on the site. A *participant* is a user who has been enrolled
in a mobile job. Users may have one or more *roles*. The most common role is ROLE_ADMIN, which gives the
user full access when they are logged in.

Self-Registration
-----------------

Users can register themselves on a site. To do so, they simply go to the site, and when prompted to
log in, click on "New User Registration". The first screen prompts them to create a username and password.

The username *must not* contain spaces or punctuation, except for "@" and "." so that email addresses can
be used as usernames.

Administrative Registration
---------------------------

Administrators can create users on the site. A user must be created before the person can be enrolled
in a specific job. An administrator can create a user by going to the "Users" menu and selecting
"Create a New User".

Self-Enrollment
^^^^^^^^^^^^^^^

A user can register a tracking device as part of their profile. All users must have an account, even if
a project is closed and the user is not allowed to log in. This allows a single record for each user so
that information like their time zone and mobile phone number do not need to be repeated throughout the
project.

Users register themselves by going to the login page

.. figure:: images/login-create-account.png

   Login Screen

Signing in with Google is trivial, and recommended since Survos Mobile also supports it, making for a very
fast login and avoiding yet another account name and password to remember. Alternatively, the user can click on
*Create sn Account* and be prompted with a screen that asks for email address, username, and password. The email and
username must be unique on the site; different users cannot have the same email. The username may be the same
as the email, which is what happens if the user registered via Google+.

Profile Editor
^^^^^^^^^^^^^^

After logging in, the user is taken to a page that allows them to complete their profile. The field details
are described in the next section, since they are a subset of the fields a project administrator will see.

The user simply fills in the fields and clicks on *Save*.

.. figure:: images/survos-profile-edit.png
   :width: 700

   Survos Profile Editor

To enroll a participant:

https://www.youtube.com/watch?v=2YmuZxtA6vY

.. toctree::
   :maxdepth: 2

   users-participants/enrolling-participants
