Inventory Project
------------------------------
**What does this project do?**

In an effort to keep track of Ethan Danahy’s office items, I created a user interface using Google Spreadsheets’ Script Editor to manage the flow of items coming in and out of his office space. The Script Editor is a very powerful tool where one can program their own, unique functions in JavaScript, making the capabilities of any spreadsheet almost limitless. By simply scanning one’s ID, the item’s barcode, and a return date, people can easily check an item in or out within seconds. The main page has many functions, including displaying the history of an item and its whereabouts, reporting a broken/missing item, adding a new item to the inventory, and searching the inventory for items.

**How to use it**

The desired process behind using this interface:
- Take the scanner and scan your item's barcode and then your own ID's barcode. Numbers will fill fields accordingly.
- Look at the labeled sheet with different return dates (barcodes encoded with "a week", "a month", "end of the semester", "6/16/17", etc) and scan return label.
- Press submit and all your information will be stored (assuming you are a returning user)

**Future of the Project**

While I spent a month working on this project, there are definitely more steps that can be taken to further the inventory system. 
- How can you make it easier to find an item if it is in a very disorganized place? Should the system know where it is supposed to go?
- How can you better deal with an item that was lost by one person, but then returned by a different user?
- When you have a kit with multiple items, should the person have to check out each individual item by hand or does the system take care of that? What if the user loses one of the individual items in the kit and the system thinks that a missing camera is actually available?
- The search function on Add page could use improvement. How can you easily get back to the main page without lots of buttons on the sheet?
- How can the user interface be made more intuitive and straightforward?
- Should the user choose a return date or should there be a return date unique to each item? (Computers can only be borrowed for a week, USB cables need to be returned by the end of the semester, etc)
- How can you make the user avoid having to click any buttons (Submit) and only need to scan?
- As a new user, it could be easier to enter new information (first name, last name, and email). It seemed to not be entirely that easy to navigate the page during a demo.
- How can you make it faster? There are many loops that the program searches through that makes it lag.

To see the Inventory Project: https://docs.google.com/spreadsheets/d/1q74d5TzMP8CcIpwsuiDnNBASyI1cfZQ8WzAVWHrKMdQ/edit?usp=sharing

Want to write your own script?
---------------------------------
**Getting Started**

Google Spreadsheets has many built in functions (like ADD(), SEARCH(), and TODAY()) that can be useful; however, there is a feature that exists in the Tools bar called the Script Editor that is much more powerful. The script editor includes special APIs to let you programmatically create, read, and edit Google Sheets, Docs, and forms. The script editor can interact with Google Sheets in two broad ways: any script can create or modify a spreadsheet if the script's user has appropriate permissions for the spreadsheet, and a script can also be bound to a spreadsheet, which gives the script special abilities to alter the user interface or respond when the spreadsheet is opened. 

**Completely New to Google Spreadsheets?**

An introduction to writing functions on the sheet: https://developers.google.com/apps-script/guides/sheets/functions
Extending functions to the script editor: https://developers.google.com/apps-script/guides/sheets

**How to Create a Google Spreadsheet with a Bound Script**
- Create a google spreadsheet: https://www.google.com/sheets/about/
- Go to Google Sheets and start a new spreadsheet
- Go to Tools in top bar, and select Script Editor…

More info about scripts bound to Google Sheets, Docs, and Forms: https://developers.google.com/apps-script/guides/bound

You can also create a standalone script: https://developers.google.com/apps-script/guides/standalone

**Web Apps**

Write a doGet(e) function, and your script editor can turn into a web app. Go into your script editor, select Publish -> Deploy as a web app... 
- https://developers.google.com/apps-script/guides/web

**Triggers**

Triggers let the script editor run a function automatically when a certain event, such as opening a document, occurs. Simple triggers are a set of reserved functions built into the script editor, like the function onOpen(e), which execute when a user opens a Google Docs, Sheets or Forms files. Installable triggers offer more capabilities than simple triggers but must be activated before use. For both types of triggers, the script editor passes the triggered function an event object that contains information about the context in which the event occurred. The e parameter, an event object, contains information about the context that caused the trigger to fire, but using it is optional. When creating your own triggered function, go to your script editor, select Resources -> Current Project’s Triggers, and from there you can add your own triggers. They can trigger when someone opens, edits, changes, or submits a form. There is also an option of having a trigger be time-drive (i.e. trigger once a day at noon).
- https://developers.google.com/apps-script/guides/triggers/

**Buttons**

In order to create a button in Google spreadsheets, you must insert a photo in a specific cell that will act as the button. Select Insert -> Image… Upload your desired image and write a function (that will trigger when the photo is selected). When you select the photo, a small box with triangle should appear in the top right corner. If you click on Assign Script and write the name of your function (without parentheses), the button will call that function whenever clicked.

**Sending Emails**

A helpful tutorial on sending emails from a Spreadsheet with a column of emails:
- https://developers.google.com/apps-script/articles/sending_emails
