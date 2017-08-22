# ReadMe #

** Plugin-Name: AccountInfoCockpit for iDempiere **

** Plug-in Version: 1.0 **

** Status: Testing **

** Licence: GPLv2 **

** Author: Patric Ma�ing (Hans Auler GmbH), Germany **

** Date: 2017 **

** Required environment: iDempiere with PostgreSQL-Database **


*ToDo: german translation*




** Description **

This plugin provides a custom form to display some special accounting information.

My decision was to create a custom form to have the full control over the functionality

and to extend the functionality step by step.
 
  
** AccountCourse **

Shows the current balance up to date at this line for the defined Account in the

defined date range. The beginning balance is on the first line showed. The 

ending balance is on the last Account posting line.


** Summary **

Shows the balance per year, month or day.


** Accountsoverview **

Displays a overview to all accounts from the COA with the current balance.

A date range can be defined in different kinds.

1. DateFrom empty and only DateTo is filled.

2. DateFrom and DateTo are inserted.

Accountvalues are not needed.

*Can be time critical if there are many data!*
 

** Accountoverview **

Displays a overview to the defined account with the current balance.

A date range can be defined in different kinds.

1. DateFrom empty and only DateTo is filled.

2. DateFrom and DateTo are inserted.



** SummaryAccountDocument **

In the most cases each product generate a separate factline. If you

have 100 positions in your invoice as example, then the view of the 

accounting for a document can be a little bit confusing. This view 

show the posting as summary per account.




** BalanceOfAccountsList **

List of all accounts in factacct with the balance for each account in the defined

time range. Also the balance before defined the time range and the ending balance.
*Can be time critical if there are many data!*



** Installation **

In the sql-folder are two files to install in the db.

1. pat_facource.sql -> Is the needed View.

2. pat_accountcourse.sql -> The function for AccountCourse




** Planed extensions **

BPartner open to defined date. What is open at time X? 

Generates Reports of the Result 

Automatic Accounting Checks - tax as example.

BPartnerCource

Show a bar graph for the accountcourse to make it easier to see deviations.




 
