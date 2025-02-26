# Things which are not solved (Software Tools)


This list is about things which could be solved in a particular
application.

For things which would require an agreement/specification see [Missing
Internet Specs](https://github.com/guettli/missing-internet-specs).


## Databases

[Mathematical equality of two SQL
statements](https://dba.stackexchange.com/questions/96865/mathematical-equality-of-two-sql-statements)

## Android Photo to Nextcloud

I take a picture with my android device. I would like to have it stored
in my nextcould account "pictures" in this schema:

> YYYY/YYYY-MM/YYYY-MM-DD

I want this to be done automatically without manual work.

## Automatically detect bottleneck of VM

Imagine an application running in a VM is too slow. You want to give the
VM more resources. But what resources are needed?

More RAM, more CPUs, faster CPU, faster disks, faster network, ...

It would be very nice if a tool could detect this by watching the app in
the VM for some time.


## Package Manager for all use cases

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

## Alternative to GSuite

GSuite is great. I have not seen a better way for:

* reading/writing mails
* Multiuser (at the same time) editing a document
* Google Slides. Very easy to use
* 15 GByte free storage
  
Related: [guettli/Microsoft-365-vs-Google-Workspace: Microsoft 365 vs Google Workspace](https://github.com/guettli/Microsoft-365-vs-Google-Workspace)

This is a bit sad, because I love open source software. But I have not seem a propriatery (or open source) alternative which is that easy to use.

BTW: In this context "easy to use" means "usable by my grandma", not "million features for geeks".
