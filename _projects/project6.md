---
layout: project
title: "Tick Data Saving Script"
description: "A Python-based automation that processes Excel data to continuously save real-time stock tick data into both an Excel file and a database, while avoiding duplicate entries."
permalink: /tickdata/
github_url: "https://github.com/superdoccimo/ayumi"  # Replace with the actual repository URL if different.
---

This project leverages Python to automate the processing of Excel data. The script reads data from a specified Excel file and automatically appends new information while avoiding duplicates. Two storage options are provided:

- **Excel File:** Save the tick data into another Excel file.
- **Database Storage:** Save the tick data into a database (e.g., MySQL, MariaDB).

Using this technology, stock tick data is recorded in real time. The script is triggered when the Excel file is saved. In conjunction with a VBA macro embedded in the Excel file—which performs periodic saves (for example, every 5 seconds)—the system continuously captures and updates the tick data.

**Prerequisites:**

- Microsoft Excel installed.
- Python installed (along with libraries such as pandas and openpyxl).
- Access to Rakuten Securities' Market Speed 2.

**Usage Overview:**

1. **File Path Configuration:**  
   Adjust file paths within the script (such as the variables for the input Excel file and the JSON output file) to match your environment.

2. **Environment Setup:**  
   Ensure that all required Python libraries are installed (e.g., by running `pip install openpyxl pandas`).

3. **Script Execution:**  
   Once configured, execute the script from your terminal or command prompt. The script will automatically read, process, and save data from the Excel file.

4. **Automated Trigger:**  
   The script is designed to run when the Excel file is saved. A VBA macro embedded within the Excel file performs periodic saves (e.g., every 5 seconds) to trigger data capture continuously.

For more detailed instructions and guidance, please refer to the accompanying blog post and YouTube video (both originally published on April 4, 2024).
