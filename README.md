# Cleaned CTFd

This fork was used in HSCTF 6, which ran during June 3-7, 2019. Changes made include:
* Team size limit of 5.
* Removed "Users" from the navbar to make room for other pages. Note that this may cause problems with CTFs running in "User" mode!
* Remove MajorLeagueCyber front-end integration.
* Modified `docker-compose.yml` to keep CTFd running locally, add multiple workers, and move the database to a separate droplet. Note: You will need to replace this file if you plan on keeping your database on the same droplet, or replace the IP!
* Modified the dynamic challenge scoring to use a sigmoidal curve instead of a parabolic curve, allowing for greater differentiation between problems with few solves.
* Added affiliation column to scoreboard.

Thanks to [CTFd](https://github.com/CTFd/CTFd) to creating a great platform!