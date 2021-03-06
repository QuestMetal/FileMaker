#File Maker Documentation#

[Q Orders](#qorders)<br>
[Inventory](#inventory)<br>
[Purchase Orders](#purchase-orders)<br>
[Reports](#reports)<br/>
[Time Cards](#time-cards)<br/>
[Charts](#charts)

#<a name="time-cards"></a> Time Cards #
## Time Card Printing ##
Time cards need to be created for the next week each Thursday. There are two different cards, (one for each shop, distinguished by MA or CU at the top of the card).

This will print a time card for each active employee in the system.

Note: This is setup to work only from the Macs and printing only to the Phaser printer.


1. Click Employee
2.	Click List View
3.	Click Print Timecards
4.	Select the Friday date you want to start timecards on
5.	Click Continue
6.	Click Print
7.	Load the timecards into the manual feed tray
timecards need to be Friday side face up with the top facing into the printer
you can stack multiple cards in the tray
be sure not to change the order of the cards once printed
8.	Once the MA cards are printed go back to your computer and click OK
9.	Click Print
10.	Manually feed the cards one at a time to the printer, Tuesday to Thursday side up.
NOTE: cards are printed in order by employee last name
11.	Go back to your computer and click OK
12.	Repeat steps 6 through 10 for the CU shop

#<a name="inventory"></a> Inventory #
##Category##
Categories are managed in the preferences are from the main menu.

1. Click preferences
2. Click Inventory Tab

To add category, scroll to the bottom and enter the category name and three letter code for the category on the last line.

Deletion of categories is not permitted.

## Stock Item Creation ##
1.	Go To Inventory
2.	Click New
3.	Enter Part Number and Description
4.	Click on Location Tab
5.	Add location(s) for the product
6.	Click Components Tab
7.	Add components to product (click Find & Add to find the components)
8.	Adjust the quantities of each component as needed
9.	Add the hours it takes to build one item.

##Stock Order Creation##

###Method 1 : The item you are building has already been setup in the inventory section.###

1.	Find the item In inventory
2.	Click on the components tab
3.	Click create stock order
4.	Enter the number of item you want to make, the system will default to the maximum stock level.
5.	Click OK

The system will now build the stock order for you. It will set the type to be stock and add all the material for that item to the Q Order material.
6.	Select which shop to build the order
7.	Print order
When the order is costed the system will automatically add the quantity made into inventory.
Removing the costed status will remove the made quantity from inventory.

###Method 2: The item you are building does not exist in inventory###
1.	Go To Q Orders
2.	Click New
3.	Click New
4.	In the company name field type Stock
5.	Click find
6.	Change Q Order Type to Stock Order
7.	Change Billing Status to Record Only
8.	Select the shop where it will be built
9.	Enter the number of hours it should take to build
10.	Enter the price for the lot in quoted amount.
11.	Add material to the Q Order (this can be done latter by layout)

##Location Setup##
To setup locations for inventory
1. Click Preferences
2. Click Inventory
3. Enter a new location on the last line
4. Select which shop this location is for

#<a name="purchase-orders"></a>Purchase Orders#

Ship To location determines which location the received products will go. Ship To location can only be changed in the PO status is open.

Click the green triangle to right of the ship to information to go to ship to location. Things like address and email address can be changed here.

#<a name="qorders"></a>Q Orders#
###Changing Shop###
Changing the shop can only be done if not material has be pulled from inventory. If you have material on the order, set the quantities to 0 then update inventory. You will then be able to change the shop.

#<a name="reports"></a>Reports#

##<a name="postingreport"></a>Posting Report##
This report prints a list of all time card entries for the day and will post the entries. 

Run this report everyday once timecards have been entered, compare this report to the timecards to ensure accurate entry.

1. Main Menu click time card data
2. Click Posting Report
3. Change the date to be the date you just entered timecards for.
4. Click Continue
5. Click Continue
6. Click Print
7. You can now compare the report to actual timecards

The report will warn you if you have not entered time for an active employee. If this is the case you will see an entry for that employee for Q# 100. You will need to adjust that entry to make it valid or delete it after entering a proper entry. Not doing so will bring up a red warning message on the main menu about rouge timesheets.  

##<a name="shopattendancereport"></a>Shop Attendance Report##
This report shows you all the hours for each shop employee split by payroll week. It shows what the expected hours are for each week. The report also shows totals for regular hours, overtime hours, absent hours, vacation hours, and WCB hours.

This report should be run at the end of every month but can be run more frequent to make error correction easier.

Monthly hours is the total of working hours plus absent and vacation hours; it excludes over time. All employees should have the same total hours.

At the end of the report there is a grand total of regular hours, overtime percentage (sum of non-adjusted overtime hours divided by grand total regular hours), absent percentage (sum of absent hours divided by grand total regular hours)

1. Main Menu click Reports
2. Click Shop Attendance Report
3. Enter / Select the Start Date (typically first of the month)
4. Enter / Select the End Date (typically last day of the month)
5. Click Continue
6. Click Print

##<a name="mnrreport"></a>Maintenance & Repair (M&R) Report##
This report shows you the time spent on maintenance and repair, it consists of two parts a printed report from FileMaker and an excel export.

The FileMaker part shows M&R time summarized by payroll week number, employee, and time factor (reg, 1.5).

The excel part consists of two sections, monthly averages and monthly totals. The monthly averages show the monthly average of M&R time for the past 10 years. The monthly totals section shows the total M&R for each month in the current fiscal year.

1. Main Menu click Reports
2. Click on the Binder tab
3. Click M&R Report
4. Enter/Select a Start date
5. Enter/Select an End date
6. Click Continue
7. Click Continue
8. Click Print
9. 	Select where to save the file and the file name
10.	Open Microsoft Excel
11.	In Microsoft Excel open the file you saved in step 9.


##<a name="salesreport"></a>Sales Report##
This report shows invoiced Q orders for the selected time period. It show total for each order and which sales person the order is for. The report also includes Sales Summary by Salesperson tab which shows total sales by sales person by month of the fiscal year. This report only generates an Excel workbook.

The report does not include record only orders (R/O).

The troi file plugin for FileMaker is required to be able to generate the report. See plugin installation.

1. Main Menu click Reports
2. Click on the Binder tab
3. Click Sales Report
4. Enter/Select a Start date
5. Enter/Select an End date
6. Click Continue
7. Select where to save the file and the file name
8. Open Microsoft Excel
9. In Microsoft Excel open the file you saved in step 7.


##<a name="supervisionreport"></a>Supervision Report##
This report shows you the time spent on supervision, it consists of two parts a printed report from FileMaker and an excel export.

The FileMaker part shows M&R time summarized by payroll week number, employee, and time factor (reg, 1.5).

The excel part consists of two sections, monthly averages and monthly totals. The monthly averages show the monthly average of M&R time for the past 10 years. The monthly totals section shows the total M&R for each month in the current fiscal year.

1. Main Menu click Reports
2. Click on the Binder tab
3. Click Supervision Report
4. Enter/Select a Start date
5. Enter/Select an End date
6. Click Continue
7. Click Continue
8. Click Print
9. 	Select where to save the file and the file name
10.	Open Microsoft Excel
11.	In Microsoft Excel open the file you saved in step 9.

##<a name="stockreport"></a>Stock Report##
This report shows all stock q orders that have been <b>loss and gained</b> during the selected date range.

1. Main Menu click Reports
2. Click on the Binder tab
3. Click Stock Report
4. Enter/Select a Start date
5. Enter/Select an End date
6. Click Continue
7. Click Continue
8. Click Print

##<a name="shoptimereport"></a>Shop Time Report##
This report consists of two parts, a FileMaker printed report and an excel report (generated as a .xml file)
Shop time is defined as time that has a shop code on it. It does not include supervision see supervision report.
The troi file plugin for FileMaker is required to be able to generate the report. See plugin installation.

1. Main Menu click Reports
2.	Click on the Binder tab
3.	Click on the Shop Time Report
4.	Enter/Select a Start date
5.	Enter/Select an End date
6.	Click Continue
7.	Click Continue
8.	Click Print
9.	Select where to save the file and the file name
10.	Open Microsoft Excel
11.	In Microsoft Excel open the file you saved in step 9.

##<a name="lossgainreport"></a>Loss/Gain Report##
This report is entirely excel based. It has 3 worksheets, Loss/Gain Summary, Loss/Gain Summary by Employee , and Loss/Gain.

Loss Gain Summary is an overall loss gain summary no details in this section.
Loss Gain Summary by Employee is a summary of Loss / Gain by employee broken down by month for the fiscal year ( based on report dates )
Loss/Gain is the detail section listing all the Loss/Gain orders, credit notes and adjustments separated by sales person.

The troi file plugin for FileMaker is required to be able to generate the report. The script will check for and if need be will install it automatically.

1. Main Menu click Reports
2.	Click on the Binder tab
3.	Loss Gain Report
4.	Enter/Select a Start date
5.	Enter/Select an End date
6.	Click Continue
7.	Select where to save the file and the file name
8.	Open Microsoft Excel
9.	In Microsoft Excel open the file you saved in step 7.

##<a name="shoppayrollworksheetreport"></a>Shop Payroll Worksheet##
This report shows the hours worked for each person in the shop for the last two weeks from the date selected. Hours are broken down by employee, week number, and position.


1. Main Menu click Reports
2. Click Weekly tab
3. Click Shop Payroll Worksheet
4. Enter / Select the last day for the payroll ( should be a Friday )
5. Click Continue
6. Click Continue
7. Select desired print options
8. Click Print

##<a name="shoppayrollexportreport"></a>Shop Payroll Export##
This report shows the hours worked for each person in the shop for the date range selected typically a two week period starting on a Friday ending on the Thursday. Hours are broken down by employee, position, and time factor for each day.

The troi file plugin for FileMaker is required to be able to generate the report. The script will check for and if need be will install it automatically.

1. Main Menu click Reports
2. Click Weekly tab
3. Click Shop Payroll Export
4. Enter / Select the start date ( should be a Friday )
5. Enter / Select the end date ( should be a Thursday )
6. Click Continue
7. Select desired filename and location to save the file
8. Click Save
9. Click Done
10. Open Microsoft Excel
11. Open the file from step 7.


#<a name="charts"></a>Charts#
##<a name="resourcesaturation"></a>Resource Saturation#
This chart shows the number of shop staff that worked for a given sales person for a given day for the last seven days. One shop person can work on multiple order throughout the day which means that they can count towards multiple sales people. A new record for the chart is created when the posting report for time cards is run.

Data comes from time cards and Q Orders. Salesperson must be selected from the 

Note: Fiscal shop orders are specifically not assigned to a salesperson on this chart.  


#Git#
git repository git://github.com/QuestMetal/FileMaker

##New Checkout##
To get an new check out:

1. go to directory
2. git init
3. git clone git://github.com/QuestMetal/FileMaker


##Update Repository##
1. git add .
2. git commit -m "message"
3. git push

##Update Local Repository
1. command prompt in the documentation directory ( C:\inetpub\wwwroot\FielMakerDocs\FileMaker )
1. git pull

Documentation Location
[http://172.16.42.86:889/FIlemakerDocs/FileMaker/FileMakerDoc.html](http://172.16.42.86:889/FIlemakerDocs/FileMaker/FileMakerDoc.html)
Be sure to click the browsers refresh button to get the latest updates
