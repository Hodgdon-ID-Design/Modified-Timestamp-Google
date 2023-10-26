# Modified-Timestamp-Google
This code was frequently employed to monitor changes made in Google Sheet rows. It was frequently integrated with other scripts and Google Sheet formulas to enhance efficiency and productivity.

# Directions

To use the provided Google Apps Script code, which automatically timestamps changes made to rows in a Google Sheets document, follow these steps:

1. Open your Google Sheets document where you want to apply this script.

2. Click on **"Extensions"** in the top menu, then select **"Apps Script."** This will open the Google Apps Script editor.

3. Delete any code that's currently in the script editor.

4. Copy and paste the provided code into the script editor.

5. Save the script by clicking the floppy disk icon or pressing **`Ctrl + S (or Cmd + S on Mac)`**.

6. Give your project a name (if prompted) and click the save button.

7. Close the script editor.

Now, every time you edit a cell in the Google Sheets document, the code will automatically timestamp the change in the corresponding cell in Column G (Column 7).

Please note the following important details about this code:

* The code timestamps changes starting from row 2 and above. If you want to timestamp changes in row 1 as well, change **`editedRow >= 2`** to **`editedRow >= 1`**

* The timestamp format is in the **`MM-dd-yyyy hh:mm:ss a`** format, which represents the month, day, year, hour, minute, second, and AM/PM.

* The code uses the time zone of the viewer. This means that the timestamp will be in the time zone of the person viewing the sheet.

* Ensure that you have edit access to the Google Sheets document where you're applying this code.

* Once you've added the code and saved it, any edits made to the sheet will trigger the onEdit function, and a timestamp will be recorded in Column G of the corresponding row.
