# README

## About

- This is phpRRDBrowse, or in short: prb -
- Author: G. Fontaine

## GPL type License
You can use it for free as long as you state the source.
See the LICENSE file

## Required software:

1. Apache
2. Mysql (if I do a db abstraction layer, you can choose any database you like.)
3. rrdtool > rrdtool-1.2.10
4. PHP with:
    - apxs
    - sigchild
    - pcntl
    - rrdtool
    - snmp
    - CLI
5. PEAR packages:
    - DB
    - XML_Parser
    * MDB2? (to be added: database abstraction layer... which one?? 
		Is it really the best way?)
6. Extras
    - Admin panel, authentication, etc...

## Installation

1. Unpack into dir
2. Edit etc/prbconfig.php
3. Create missing dirs (log, rrd, www/png)
4. check file access mods (webserver must write in rrd, log and www/png)
5. create prbdb database in mysql (use prbsql.txt)
6. Setup crontab to poll every 5 mins with prbupdated

## Features:
- browse by OS, vendor, location
- host filter
- host and module Info box with editing
- custom sql views
- editing of info records
- look and feel customisable via css stylesheet
- simple polling performance statistics

## Todo: 
- installation script
- improve host discovery and add manual host configuration for
    none snmp enabled hosts
- documentation
    installation guide
    user manual
    developpers guide (module dev how-to)

## More stuff to add:
- form validation
- users, authentication and user management
- database abstraction layer
- templates (css based)
- labels
- advanced search
- error logging to file or database
