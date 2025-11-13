# **Browser Table Tools**

A simple, 100% in-browser web application to perform SQL-like operations (Append and Join) on your local .csv, .xls, or .xlsx files.

This tool runs entirely in your web browser. No data is ever uploaded to a server, ensuring your data remains private and secure on your own computer.

## **Features**

* **Purely Client-Side:** All processing is done locally using JavaScript.  
* **No Data Upload:** Your files never leave your machine.  
* **File Support:** Reads .csv, .xlsx, and .xls files.  
* **SQL-like Operations:**  
  * **Append (Union):** Stacks two tables on top of each other.  
  * **Inner Join:** Combines rows from two tables based on a common key, including only rows that match in both tables.  
  * **Left Join:** Includes all rows from the left table, and matching rows from the right table.  
  * **Right Join:** Includes all rows from the right table, and matching rows from the left table.  
  * **Outer Join:** Includes all rows from both tables, with null values where no match is found.  
* **Result Preview:** View the first 100 rows of your result directly on the page.  
* **Export Results:** Download the complete merged/appended table as a new .xlsx file.

## **How to Use**

1. **Open the Application:** Simply open the table\_tools.html file in any modern web browser (like Chrome, Firefox, Safari, or Edge).  
2. **Upload Files:** Click the file input area to select, or drag-and-drop, one or more files you want to work with. The tool will parse them and list them.  
3. **Choose Operation:** Select the operation you want to perform (e.g., "Left Join") from the dropdown menu.  
4. **Configure Operation:**  
   * **For Append:** Select the two tables you want to stack.  
   * **For Join:** Select the Left Table, Left Key (the column to join on), Right Table, and Right Key. The key dropdowns will populate automatically after you select a table.  
5. **Run Operation:** Once configured, click the "Run Operation" button.  
6. **Preview and Download:** The application will process the data and display a preview. You can then click the "Download as .xlsx" button to save your new file.

## **Technologies Used**

* **HTML:** For the application structure.  
* **Tailwind CSS:** For styling the user interface.  
* **SheetJS (xlsx.js):** A powerful library for reading, parsing, and writing spreadsheet files in the browser.