giveandtake
===========

Give and Take Command at NERSC


Versions
--------

give/take:    Standard give & take. (Give to one user, take based on username).

givemessage:  give + quiet and message modes.
                Includes options to not send an notification email (-q)
                or add a message to the notification email (-m "<message>").
 
giveusers:    givemessage + can give to multiple users

                 e.g. give -u userA -u userB -u userC -u userD ....

              Sends files to all users up to a specified limit. Checks for and
                 ignores invalid users and duplicated usernames. Sends same
                 notification email (or no email) to all users.

givegroup:    givegroup + can give to permissions groups

                 e.g. give -u userA -g groupA -u userB -g groupB -g groupC

              Sends to all specified users in users in permissions groups up to
                 a specified global limit. If combined number of users is
                 exceeded, give exits. Checks for an ignores invalid users and
                 duplicated usernames to allow overlapping permissions groups. 
