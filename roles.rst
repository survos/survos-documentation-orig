======================
Account Roles
======================

*ROLE_PARTICIPANT*
------------------------------------

Participants are study subjects in a study.  They have a unique anonymous identifier.


*ROLE_OWNER*
------------------------------------

Owner accounts have full access to configure and edit a study.  They also have full access to PII.
Their account identifier (username) is identifiable, even if they are participating as a study participant (usually for testing)


*ROLE_RESEARCHER*
------------------------------------

Researchers have read-only access to the entire study design and data, EXCEPT PII of the participants.
Their account identifier (username) is identifiable, even if they are participating as a study participant (usually for testing)


*ROLE_APPLICANT*
<<<<<<< HEAD
------------------------------------

Applicants are not yet in the study, and have no study identifier.  They are not eligible to be enrolled
in any waves except screener waves, which are used to determine if they are eligible for the study.

=======
    Applicants are not yet in the study, and have no study identifier.  They are not eligible to be enrolled
in any waves except screener waves, which are used to determine if they are eligible for the study.
>>>>>>> 33e064430e0b8f0afb7d2cef31f36fdd30446c0d

*ROLE_FIELD_WORKER*
------------------------------------

roles.ROLE_FIELD_WORKER

*ROLE_TURKER*
------------------------------------

For organizing crowdsourced results, a turker automatically creates an account.  They do not have a study
identifier, but they do have an independent (and anonymous) Turker code.





