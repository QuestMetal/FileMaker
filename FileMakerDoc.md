#File Maker Documentation#

Q Orders<br>
Inventory<br>
Purchase Orders

# Time Cards #
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

# Inventory #
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

#Purchase Orders#

Ship To location determines which location the received products will go. Ship To location cna only be changed in the PO status is open.

#Q Orders#
###Changing Shop###
Changing the shop can only be done if not material has be pulled from inventory. If you have material on the order, set the quantities to 0 then update inventory. You will then be able to change the shop.

#Reports#
##Shop Time Report##
This report consists of two parts, a FileMaker printed report and an excel report (generated as a .xml file)
Shop time is defined as time that has a shop code on it. It does not include supervision see supervision report.
The troi file plugin for FileMaker is required to be able to generate the report. See plugin installation.

1. Main Menu click Reports
2.	Click on the binder tab 
3.	Click on the Shop Time Report
4.	Enter/Select a start date
5.	Enter/Select an End date
6.	Click Continue
7.	Click Continue
8.	Click Print
9.	Select where to save the file and the filename
10.	Open Microsoft Excel 
11.	In Microsoft Excel open the file you saved in step 9.

#Push Changes To Git#
git repository git://git.com/QuestMetal/FileMaker


1. git add .
2. git commit -m "message"
3. git push


