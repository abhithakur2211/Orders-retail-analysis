# Orders-retail-analysis
This Python script performs an ETL process for retail order data. It downloads the dataset from Kaggle, extracts it, and loads it into a DataFrame. The script cleans and transforms the data by handling null values, renaming columns, deriving features, and dropping unnecessary columns, then loads it into SQL Server.

The uploaded file is a Python script that analyzes and processes order data. Here’s a concise description of its functionality:

1. **Data Download and Extraction**: Downloads a retail orders dataset from Kaggle and extracts it from a zip file.
2. **Data Cleaning**:
   - Reads the dataset and replaces specific values with `NaN` for handling missing data.
   - Renames columns to lowercase and replaces spaces with underscores.
3. **Feature Engineering**:
   - Derives new columns such as `discount`, `sale_price`, and `profit`.
   - Converts the `order_date` column to a datetime format.
4. **Data Modification**:
   - Drops unnecessary columns like `list_price`, `cost_price`, and `discount_percent`.
5. **Database Upload**:
   - Connects to an SQL Server database using SQLAlchemy.
   - Uploads the processed data to a table named `df_orders` using the "append" option.

