Things which are not solved yet
###############################


Python
======

Python is great for backend stuff. For example the Django web framework.

But up to now you can't write python code which gets executed in the web browser. There are some solutions, but they are not wide spread yet.

Databases
=========

`Mathematical equality of two SQL statements <https://dba.stackexchange.com/questions/96865/mathematical-equality-of-two-sql-statements>`_



Django
======

Web-GUI for installing apps. No editing of python files to install an app. Nextcloud is great here. You can upgrade from one version to the next via web gui. This is great.

Performance Analysis
====================

A tool like new relic (low overhead sampling profiler that collects call graphs for running production apps), but open source. 

These look good: https://github.com/benfred/py-spy

And: https://github.com/uber/pyflame


Android Photo to Nextcloud
==========================

I take a picture with my android device. I would like to have it stored in my nextcould account "pictures" in this schema: 

    YYYY/YYYY-MM/YYYY-MM-DD

I want this to be done automatically without manual work.

Automatically detect bottleneck of VM
=====================================

Imagine an application running in a VM is too slow.
You want to give the VM more resources.
But what resources are needed?

More RAM, more CPUs, faster CPU, faster disks,
faster network, ...

It would be very nice if a tool could detect this
by watching the app in the VM for some time.


Creating group in email, easy like in WhatsApp
==============================================

Creating a new group for email communication should
be as easy as in WhatsApp.

From email address to profile image
===================================

Unfortunately it is not possible up to now to combine an email address with
a profile image.
For example your mail is mr.bean@example.com and you want to make a photo available
to make everyone smile (https://www.google.de/search?tbm=isch&q=mr+bean) ... AFAIK
there is no way to publish this, and of course no other way of people who have your
email address to find this image.

JSON
====

Store binary data in json.

Schemas for json. AFAIK there is not established solution.

JSON has no date/datetime data type: https://stackoverflow.com/questions/10286204/the-right-json-date-format
You can use this: "2012-04-23T18:25:43.511Z". But how to distinguish a string which is exactly "2012-04-23T18:25:43.511Z" from a string
which should be a datetime?

JSON has no timedelta data type.

Syncing Nextcloud without GUI
=============================

I know the nextcloudcmd, but this is only a command, not a daemon.

There needs to be a daemon which detects (and syncs) changes immediately (using inotify).

Related: https://help.nextcloud.com/t/sync-without-gui-but-live-inotify/49420

PostgreSQL
==========

Automaticaly detect which indexes are missing or "not needed". Some kind of clever tool could analyze the work-load for some days and adapt the indexes (or at least provide some suggestions)

Package Manager for all use cases
=================================

rpm and dpkg are used at the "root" level.

But most programming languages re-invent package management and dependency resolution for their environment: 

* pip for python
* npm for JavaScript
* gem for ruby
* ...

I think (and hope) sooner or later there will be **one** package manager. Just like git has won the "which version control system is best" battle.




