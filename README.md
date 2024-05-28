# UpdateServersPlaybook

This is a quick Ansible Playbook that I wrote to update my Debian/Ubuntu based VPS boxes out on the internet. I was tired of having to login and update things or make sure they rebooted even though I have them set to "auto update". Sometimes that wasn't working... I blame the administrator (me)... 

# What does this do?

It logs into your servers after asking for the ``sudo`` password for the user, updates that ``apt cache`` then runs the update and upgrade functions. After that completes, it checks for the file that screams if a reboot is necessary. If found, it processes a clean reboot proceedure.

# TODO

Add support for RPM based systems as soon as I have some that I'm using for daily driving.


# Licence

Licenced under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/). Do what you want with the code but remember to respect the Ansible, Linux, and distro specific licenses as well.
