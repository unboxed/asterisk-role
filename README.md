asterisk-role
========

This role will download and install [Dahdi][], [Libpri][] and [Asterisk][] and start [Asterisk][] running on an Debian-based installation.

***

### Usage

To include this role, please use include this command in the roles section of the playbook

> { role: asterisk }

***

### Variables

Declaring the following variables in the using playbook will specialise the configuration of the [Asterisk][] installation.

* **global-asterisk-group** will assign Asterisk to the given group, and assign all configuration and logging file read/write/execute access for that group.
* **global-config-dir** will set the filepath of the directory that [Asterisk][] will store its configuration files in. This defaults to */etc/*.
* **global-log-dir** will set the filepath of the directory that [Asterisk][] will send its logfiles to. This defaults to */var/log/*
 
Please note - due to the limitations of markdown, the variables above are actually incorrect. In each case, please replace the hypen (**-**) with an underscore (**_**).

[Asterisk]: http://www.asterisk.org/ "Asterisk"
[Dahdi]: http://www.asterisk.org/downloads/dahdi "Dahdi"
[Libpri]: http://www.asterisk.org/downloads/libpri "Libpri"