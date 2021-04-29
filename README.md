# LR-SMBClientSecurity-MPE
LogRhythm MPE Rule for the Microsoft-Windows-SMBClient/Security EventLog
  
This is a single base rule, with one sub-rule. I have only observed event IDs 31010 (insufficient access rights) and 31001 (invalid credentials) being logged.  
Upon import, a new log source type called "MS Win Event Log XML - SmbClient Security" will be created, with the abbreviation "WinEvtX - SmbClntSec" and log source type ID 1000000014. Any conflicint log source type with that ID will be overwritten.  
  
NB: This rule has MPE Rule IDs 1000000212 and 1000000213, and MPE Base Rule Regex ID 1000000055. Be sure that you don't have rules with conflicting IDs before you import this rule.
