asterisk-role
========

This role will download and install [Dahdi][], [Libpri][] and [Asterisk][] and start [Asterisk][] running on an Debian-based installation.

***

### Usage

To include this role, please use include this command in the roles section of the playbook

    { role: asterisk }

***

### Variables

Declaring the following variables in the using playbook will specialise the configuration of the [Asterisk][] installation.

* **global\_asterisk\_group** will assign Asterisk to the given group, and assign all configuration and logging file read/write/execute access for that group.
* **global\_config\_dir** will set the filepath of the directory that [Asterisk][] will store its configuration files in. This defaults to */etc/*.
* **global\_debug** when set to _True_ this will switch on tasks that start and stop Asterisk processes. If not defined, this defaults to false.
* **global\_log\_dir** will set the filepath of the directory that [Asterisk][] will send its logfiles to. This defaults to */var/log/*
 

[Asterisk]: http://www.asterisk.org/ "Asterisk"
[Dahdi]: http://www.asterisk.org/downloads/dahdi "Dahdi"
[Libpri]: http://www.asterisk.org/downloads/libpri "Libpri"