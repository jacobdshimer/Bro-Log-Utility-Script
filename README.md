# Bro-Log-Utility-Script

This script will allow you to slice different types of Bro Logs for better data analysis.  Currently you can only combine multiple log files together into one file, slice a log based off of the fields, slice a conn.log based off of the port and run multiple PCAPs against the Bro IDS.

Initial Push 0.1 - September 29, 2017
Created the bro_utility.py, combiner.py, fields.py, and portslicer.py

Update 0.1.1 - October 12, 2017
Created Bro.py

Update 0.1.2 - November 17,2017
Updated Bro.py - Fixed a problem where the "combined_" file would get repeated over and over again.  Also fixed where if, for example, only one HTTP.log, it would be repeated over and over again in the "combined_http.log" instead of only copying it once.  This was done by deleting the logs that were dropped by Bro after they were created.
