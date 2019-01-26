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




