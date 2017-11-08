# cthulhu
A BaSH front end to mtglacier perl AWS Glacier tool

Ph'nglui mglw'nafh Cthulhu R'lyeh wgah'nagl fhtagn 
Reference to mtglacier --> https://github.com/vsespb/mt-aws-glacier

Version 1.3_1 - Wed Nov  8 08:08:58 CET 2017
            Added a clarification on how writeToMainLog and useSystemLog do interact

Version 1.3 - Mon Oct 30 15:09:31 CET 2017
            
            Added support for configuration file 
            Added action to remove all items from a vault (purge) 
            Added action to delete a purged vault 
            Added install action, to be execute as first run 
            Added support for syslog 

Version 1.2 - Tue Sep 12 08:33:49 CEST 2017
            
            Added check if the target directory exists
            Fixed exit code in check-status to be unique

Version 1.1 - Mon Sep  4 11:14:54 CEST 2017
            
            Changed sync action log to record the target vault
            Changed check actions log to record the target directory (as no vault is passed to the command)

Version 1.0 - Fri Sep  1 14:22:02 CEST 2017

Set the following variables to achieve batch usage behavior (e.g. via crontab only)
            
            logActionsToFile=1
            quietMode=1
            writeToMainLog=1

Set the following variable to achieve interactive usage (e.g. for shell calls only)
            
            logActionsToFile=0
            quietMode=0
            writeToMainLog=0
