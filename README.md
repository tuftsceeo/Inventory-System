Inventory Project Documentation
------------------------------

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

