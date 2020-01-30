# BackupRotation

A lightweight BASH backup rotation script built to take arguments or an ini file 

This can do daily, weekly, monthly, and yearly (annual) backup retention. It will keep the number of days/weeks/months/years as specified in the INI file or commandline arguments.

A run with no arguments will look for an INI file in /etc/defaults called BackupRotated.ini

This allows the script to simply be symlined linked (or placed) in cron.daily for easy automation 

The scrit has a default expection to simply GZIP the source into the destination. but the command can be overridden on some or all of the backups using commandline aguments or the INI file. Any special characters in the command will need to be propery escaped. 
