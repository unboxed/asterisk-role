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
* **global\_log\_dir** will set the filepath of the directory that [Asterisk][] will send its logfiles to. This defaults to */var/log/*
