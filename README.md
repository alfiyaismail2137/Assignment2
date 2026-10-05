# Assignment2
Data Cleaning and transformation
# 1) Handling Missing Values:
   • Check for missing values in the 'Price' column. How would you handle products with missing price information?
      <br>find median and median through following steps :
      select price column --> Transform-->Statistics-->Median.
      Transform-->Replace values
      Missing value replaced by Median value 130.
   <br>• If there are products with missing categories, propose a strategy to impute or deal with these missing values effectively.
     <br>Select Category column-->Transform-->Replace Value-->Unknown.
# 2) Correcting Inconsistent Data:
    • Identify any inconsistent text formats present in the "Product Name" column.

    • Identify any typos present in the "Category" column.
    • Use the find and replace function to standardize the text formats in the "Product Name" column and fix any typos or misspellings in the "Category" column.
# 3) Removing Duplicates:
   • Identify any duplicate rows within the dataset based on the entirety of each row, and remove them if any.
# 4) Splitting and Merging Data:
   • Split the "Product ID" column into two separate columns for " Manufacturing Date" and "Country Code". Remove unnecessary characters, if any.
   • Merge the "Brand Name" and "Product Name" columns into one column named "Product Brand".
   # 5) Number Formatting:
   • Format the data type of the "Price" column to currency format. 
   • Format the "Manufacturing Date" column to display dates in the "DD-MM-YYYY " format. 
  # 6) Conditional Formatting:
   • Apply data bar or color scales conditional formatting in the "Price" column.
   • Create a custom rule for conditional formatting in the "Category" column to highlight cells where the category is "Electronics."
   
