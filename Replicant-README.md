Replicant
=========

About
-----

Replicant is a fully free Android distribution running on several devices.
It is based on CyanogenMod and thus on the Android Open Source Project.

Android includes software from various sources, released under different free software licenses.
Replicant attempts to remove or replace any non-free component (running on the main CPU) that is needed by Android, whenever this is possible.

We are not experts in embedded devices, just a couple enthusiastic hackers that are giving a try.

Credits
-------

Replicant is based on CyanogenMod <http://www.cyanogenmod.com/> which is based on the Android Open Source Project <http://www.android.com/>. 

Contributors
------------

The full list of contributors to the Replicant code base must be very long since it is based on CyanogenMod and AOSP, which are both using third party projects.
However, a (non-exhaustive) list of people who specifically contribute(d) to Replicant is available at: <http://redmine.replicant.us/projects/replicant/wiki/People>

Artwork copyright
-----------------

Copyright 2011 Mirella Vedovetto
Copyright 2012 Paul Kocialkowski

This work is licensed under the Creative Commons Attribution-ShareAlike 3.0 Unported License. To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/3.0/ or send a letter to Creative Commons, 444 Castro Street, Suite 900, Mountain View, California, 94041, USA.

Links
-----

Website: <http://www.replicant.us/>
Wiki/Tracker: <http://redmine.replicant.us/>

CyanogenMod
===========

Submitting Patches
------------------
Patches are always welcome!  Please submit your patches via CyanogenMod Gerrit!
You can do this by using these commands:

    (From root android directory)
    . build/envsetup.sh
    (Go to repo you are patching, make your changes and commit)
    cmgerrit <for(new)/changes(patch set)> <branch/change-id> 

    repo start cm-10.1 .
    (Make your changes and commit)
    repo upload .
Note: "." meaning current directory
For more help on using this tool, use this command: repo help upload

Make your changes and commit with a detailed message, starting with what you are working with (i.e. vision: Update Kernel)
Commit your patches in a single commit. Squash multiple commit using this command: git rebase -i HEAD~<# of commits>

To view the status of your and others' patches, visit [CyanogenMod Code Review](http://review.cyanogenmod.org/)


Getting Started
---------------

To get started with Android/CyanogenMod, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

To initialize your local repository using the CyanogenMod trees, use a command like this:

    repo init -u git://github.com/CyanogenMod/android.git -b cm-10.1

Then to sync up:

    repo sync

Please see the [CyanogenMod Wiki](http://wiki.cyanogenmod.org/) for building instructions.

For more information on this Github Organization and how it is structured, 
please [read the wiki article](http://wiki.cyanogenmod.org/w/Github_Organization)

Buildbot
--------

All supported devices are built nightly and periodically as changes are committed to ensure the source trees remain buildable.

You can view the current build statuses at [CyanogenMod Jenkins](http://jenkins.cyanogenmod.org/)
