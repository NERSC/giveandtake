giveandtake
===========

Give and Take Command at NERSC


Versions in repository:

give & take: Original versions (Aug 1, 2017)

givemessage: Adds -q (Quiet mode: no email).
             Adds -m (Message: add a message to the email).

giveusers:   givemessage + can give files to multiple users with multiple -u's.

             e.g. -u kngott -u tkoskela -u jdeslipp

             Checks for whether users are valid & removes duplicates before 'give'ing.
             Includes variable to limit total number of users allowed in one give command. 
 
givegroup:   giveusers + can give to multiple dependency groups with -g

             e.g. -g staff -u kngott -g m1881 -u tkoskela ...

             Total # of users across all -g's and -u's limited by admin defined variable.
             Includes blacklist to prevent giving to admin or other sensitive permissions groups.
