Things which are not solved yet
###############################


Python
======

Depedency Management. The tool pip works somehow, but a real dependency management is missing.


`Configuring the logging of a third party script <https://stackoverflow.com/questions/29962525/configuring-the-logging-of-a-third-party-script>`_

I was told the tool `poetry <https://github.com/sdispater/poetry>`_ does solve this, but I have not tried it yet.

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
