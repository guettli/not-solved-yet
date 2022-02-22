Things which are not solved (Software Tools)
============================================

This list is about things which could be solved in a particular
application.

For things which would require an agreement/specification see [Missing
Internet Specs](https://github.com/guettli/missing-internet-specs).

Python
------

Python is great for backend stuff. For example the Django web framework.

But up to now you can't write python code which gets executed in the web
browser. There are some solutions, but they are not wide spread yet.

Compiling Libraries for Python
------------------------------

If you install a package which needs compiling, then it is likely that you get an error like this

```
    In file included from psycopg/adapter_asis.c:28:
    ./psycopg/psycopg.h:36:10: fatal error: libpq-fe.h: No such file or directory
       36 | #include <libpq-fe.h>
```

With the help of your favorite search engine you usualy find the needed command to fix this.

For example `sudo apt install libpq-dev`.

It would be great if this manual step could be automated, so that the missing library gets installed automatically.


Databases
---------

[Mathematical equality of two SQL
statements](https://dba.stackexchange.com/questions/96865/mathematical-equality-of-two-sql-statements)

Django
------

Web-GUI for installing apps. No editing of python files to install an
app. Nextcloud is great here. You can upgrade from one version to the
next via web gui. This is great.


Extending Django models via the admin interface.
This would be cool. AFAIK you can do this in ERPNext.
But this uses the Frappé framework, not Django.
Adding new columns via admin interface would make
Django a low code framework.

Performance Analysis
--------------------

A [Statistical Profiler](https://en.wikipedia.org/wiki/Profiling_(computer_programming)#Statistical_profilers) like new relic, but open source.
There are tools (for example [py-spy](https://github.com/benfred/py-spy) and [speedscope](https://github.com/jlfwong/speedscope)) but up to now there is no framework which works for several langnuages. Maybe [Parca](//parca.dev) will solve this.

Maybe [Jaeger](https://github.com/jaegertracing/jaeger) could get used. But up to now Jaeger does only create traces for the service calls, not the method calls of an application.

Android Photo to Nextcloud
--------------------------

I take a picture with my android device. I would like to have it stored
in my nextcould account "pictures" in this schema:

> YYYY/YYYY-MM/YYYY-MM-DD

I want this to be done automatically without manual work.

Automatically detect bottleneck of VM
-------------------------------------

Imagine an application running in a VM is too slow. You want to give the
VM more resources. But what resources are needed?

More RAM, more CPUs, faster CPU, faster disks, faster network, ...

It would be very nice if a tool could detect this by watching the app in
the VM for some time.

Syncing Nextcloud without GUI
-----------------------------

I know the nextcloudcmd, but this is only a command, not a daemon.

There needs to be a daemon which detects (and syncs) changes immediately
(using inotify).

Related:
<https://help.nextcloud.com/t/sync-without-gui-but-live-inotify/49420>

PostgreSQL
----------

Automaticaly detect which indexes are missing or "not needed". Some kind
of clever tool could analyze the work-load for some days and adapt the
indexes (or at least provide some suggestions)

Package Manager for all use cases
---------------------------------

rpm and dpkg are used at the "root" level.

But most programming languages re-invent package management and
dependency resolution for their environment:

- pip for python
- npm for JavaScript
- gem for ruby
- helm charts for Kubernetes
- ...

I think (and hope) sooner or later there will be **one** package
manager. Just like git has won the "which version control system is
best" battle.

Related: https://github.com/guettli/django-and-third-party-js
