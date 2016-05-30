# Document ConfigMgr

This repo is being maintained by Ryan Ephgrave (Ryan2065). If you have any suggestions, feel free
to post on GitHub or reach me on Twitter @EphingPosh

## Requirements

* SCCM 2012
    * Should work with 2012 RTM - Current Branch
* Word 2010 - 2016
* PowerShell 3.0

## Instructions

This script does not rely on the ConfigMgr cmdlets, so it will work on RTM - Current Branch. 
You can also run it on a computer that is not on the domain by using:

runas /netonly /noprofile /user:domain.fqdn\username PowerShell.exe

Then simply run the script like you would normally!

Script has great documentation on all the parameters and examples.

## To Do:
* Offline support
    * Run from a computer without Word (say, the CM server) and store results in JSON.
* Compare different states
    * If offline support exists and the results are stored in JSON, those results could be used
    to compare previous state of the CM environment to the current state.
* Optimize code
    * The code currently queries the same things multiple times. It could be highly optimized
* Give your suggestions in the comments!