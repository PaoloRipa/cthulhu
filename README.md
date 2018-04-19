# cthulhu
A BaSH front end to mtglacier perl AWS Glacier tool

> Ph'nglui mglw'nafh Cthulhu R'lyeh wgah'nagl fhtagn 

Reference to mtglacier --> https://github.com/vsespb/mt-aws-glacier

## Changelog

[Version 2.0](https://github.com/PaoloRipa/cthulhu/milestone/1) - Thu Apr 19 19:47:37 CEST 2018

            Issue #2 Add action specific help messages
            Issue #3 Expand add-schedule action to allow scheduling other types of actions 
            Issue #4 Rename schedule-sync to add-schedule 
            Issue #6 Add del-schedule action 
            Issue #7 Harmonize code
            Issue #8 Add action to print exit codes reference information 
            Issue #10 Port fix for Issue #9 
            Issue #11 Port fix for Issue #1 
            Issue #12 Add details on archive status to check-status help 
            Issue #13 Improve check-status action to send reports via email 
            Issue #14 Formatting issues with emails sent from checkDirectory 
            Issue #16 Add sync-mtime action
            Issue #17 Add sync-thash action 
            Issue #18 Improve show-schedule output message 
            Issue #19 Add an actions to retrieve files from a vault 
            Issue #20 restore-prepare: email reminder not sent at planned time blocker 
            Issue #21 del-schedule garbage output when deleting a check-status action blocker 
            Issue #22 del-schedule action confirmation message always refers to sync actions 
            Issue #23 Add CLI flag to show version 
            Issue #24 Add show-conf action 
            Issue #25 Implement action auto-completion
            Issue #26 Naming for sync-mtime and sync-thash log files conflicts with check-sync action
            Issue #27 Missing -v flag in help page
            Issue #28 Change default main log name
            Issue #29 Specify human readable format in list-vaults action
            Issue #30 Implement journal recovery action(s)
            Issue #31 Autcompletion not working outside of $HOME

Version 1.6 - Thu Feb 15 11:05:48 CET 2018

            Added function to list scheduled sync actions
            Forced interactive mode now disables sending emails
            Fixed check-sync function to send email only if enabled by config
            Added support for CLI flags
            Added CLI flag to force interactive mode
            Added batch/interactive usage configs to help file and to main configuration file
            checkDirectory action logic has been made filesystem agnostic
            checkDirectory action now sends email alerts for scheduled batch actions
            Fixed error message in checkDirectory action
            checkDirectory action can now log action being aborted
            Revised and expanded online help
            Added CLI flag to show help (for compatibility)
            Improved email generation, now supporting plain text basic formatting (newlines, tabs...)
            Added fix for issue #1
            Added fix for issue #15

Version 1.5 - Mon Feb 12 15:48:25 CET 2018 

             Minor "cosmetic" fixes from previous versions
             Added function to upgrade the configuration file 
             Enhanced install gen-conf to add mtglacier directory to PATH 
             Added version number that is displayed by main help function
             Fixed a formatting bug in printMsg function, causing special chars to be interpreted
             Added a function to schedule sync actions via crontab 

Version 1.4 - Thu Nov 9 10:53:34 CET 2017

             Added support to send out emails
             Added success check at the end of sync action
             Added checks against required dirs and files
             Added function to check last execution of sync action
             Added configuration variable to disable check at the end of sync action
             Added function to generate a test email

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

### Roadmap

[Version 2.0](https://github.com/PaoloRipa/cthulhu/milestone/1)

[Unscoped](https://github.com/PaoloRipa/cthulhu/milestone/2)