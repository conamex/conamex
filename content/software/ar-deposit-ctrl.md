---
title: AR Deposit Ctrl
---

* Do we require our own security for users to login and access this program?
* The user will go into the option ISV to Sage Transfer
* The user will have a grid that will allow them to transfer 1 or more D&M batches to the GL that they can choose.
    * The batches available to transfer will be based on ISV status fields being
    used to indicate their current status. Only those marked available to transfer
    will be shown for the user to choose from.
    * Multiple batches transferred can be transferred into 1 GL Batch, reducing
    the number of GL batches created based on a 1-1 transfer.
    * There are options to be reviewed here, as to if we are supporting multiple
    companies initially and letting the program manage the transfer and sorting
    of data to multiple companies at once or if user must choose the company 1st
    to then choose only the batches available for that company. More manual
    requirements as number of companies and volumes increase.

* Modifications to existing and within existing ISV software to
perform the following maintenance requirement. Mapping information based on:
    * Company to Sage Company DB
    * Currencies
    * Linking Country/Branches/Locations to GL accounts
    * Does/Should the Donation software and later membership software
    perform as their own A/R system with all deposits/payments being
    processed to go to GL, or do we submit all via Sage AR – topic to
    be discussed as needed.
* Extracting the data from the ISVSoftware processes – including into
their own batch/entry tracking systems.
    * Define the extracting criteria – date/ date range etc.
    * The level of tracking and integrating possible requires that
    the foundation within D&M Software is created and developed accordingly
    * Usually done in two steps:
        * Extract data and place in a table to show the raw details used to be transferred
        * Consolidated table if required to only transfer the minimum amount
        of data to Sage 300 (especially if D&M software is doing the A/R functions)
        * Define the consolidating criteria to be used
* Batch/Entry Tracking System
    * Deposit Batches: Shows all the deposit data available to be transferred, users have different options to view based on status field and year, etc.
    * The goal should be a full financial (AR) module that all D&M software feeds into.
    * All deposit batches above, unless a user requires to enter certain payments manually are all automatically generated as users perform operations requiring financial transactions.
    * As for all payments, donations, membership renewals that are done via
    internet they are again automatically generated and maintained per client
    requirements based on triggers. For example as donations come in, the 1st
    donation of the day creates a batch for that day and then all the future
    transactions for that day get added automatically to the deposit batch for
    that date per configuration and until the cutoff for that day and then the
    next transaction after the cutoff date automatically creates a new deposit
    batch for the new date.
    * Based on this logic, the only user interaction is to view, print (audit purposes), verify the batch and validate/post it.
    * There is an assortment of reporting that can be printed based on this information, auditing purposes and full verifications between software and banking institution if all is setup and developed accordingly to the company needs..
* Transfer to Sage 300 A/R or G/L
    * The user has the ability to transfer deposit batches on a 1 to 1 basis or create a transfer batch of multiple deposit batches to be transferred in one step.
    * In the case of the TTC, the ability to a later date control transferring deposit/transfer batches to multiple companies within the Sage environment.
* The transfer function will automatically create one or more GL batches based on what is decided and for which the user transfers to GL.
    * It will then return to D&M software (within their deposit control system) the reference information from Sage 300 as available and possible according to decisions to be made for full tracking and auditing.
    * For example:  A D&M Batch might be # 1001 the Transfer process will return and update D&M Batch 1001 with what might be GL Batch 2005 so full references between systems are tracked.
* Other Assistance Available to Work in Configuration and Setup of Servers (windows and SQL for best performance and redundancy for mission critical requirements.
* SQL reporting services setup and designing of reports per purposes required including auditing and verifications and using data from D&M software/Sage 300 Software and other, including such things as summary reports over multiple modules and companies.
* Financial consolidation auditing verifications between D&M software and TTC financial institution
