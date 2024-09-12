# PySpark JSON/CSV File Handling on Databricks

This project demonstrates how to handle **JSON** and **CSV** files using **PySpark** on **Databricks**. The tasks involve reading data, displaying content and schema, and saving the output in multiple formats such as JSON, Parquet, and Delta.

## Files in this Project:
- `file_handling_example.py`: Contains the PySpark code for file handling on Databricks.
- `README.md`: This documentation file.

## Steps Covered:

1. **Loading a JSON file into a DataFrame**:
    - Read a JSON file from the specified path in Databricks.
    - Show the contents of the DataFrame.
    - Print the schema of the DataFrame.
    - Save the DataFrame back as a JSON file.

2. **Loading a CSV file into a DataFrame**:
    - Read a CSV file with header and schema inference options enabled.
    - Show the contents of the DataFrame.
    - Print the schema of the DataFrame.
    - Save the DataFrame as **Parquet** and **Delta** files in Databricks.

## Instructions:

1. **Set Up in Databricks**:
    - Ensure that your Databricks environment has PySpark configured.
    - Update file paths in the script (`file_handling_example.py`) to match your Databricks FileStore (e.g., `/FileStore/tables/`).

2. **Running the Code**:
    - Upload the script to your Databricks workspace.
    - Execute the script in a Databricks notebook.

3. **Output**:
    - The script will output:
        - A new JSON file after reading from the initial JSON file.
         ![image](https://github.com/user-attachments/assets/dc024bc0-89f9-4406-a61c-ba9288c80751)

        - A **Parquet** file and **Delta** table after processing the CSV data.
          
          ![image](https://github.com/user-attachments/assets/603e60eb-d33d-4f4d-a857-0b43ad3b7346)


## Notes:
- The Delta format requires **Delta Lake** to be enabled in your Databricks environment.
- The script uses the `overwrite` mode, ensuring that existing files are replaced. Modify as needed for different behavior.
- This project is tailored for Databricks and is designed to work with Databricks FileStore paths.

---

This project serves as a basic example for handling JSON and CSV files using PySpark on Databricks, showcasing how to work with structured data and store it in different formats.
