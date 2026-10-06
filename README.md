# Assignment2
Data Cleaning and transformation
# 1) Handling Missing Values:
   • Check for missing values in the 'Price' column. How would you handle products with missing price information?
      <br>Find median  through following steps :
      <br>select price column --> Transform-->Statistics-->Median.
      <br>Transform-->Replace values.
      <br>Missing value replaced by Median value 130.
   <br>• If there are products with missing categories, propose a strategy to impute or deal with these missing values effectively.
     <br>Select Category column-->Transform-->Replace Value-->Unknown.
# 2) Correcting Inconsistent Data:
   • Identify any inconsistent text formats present in the "Product Name" column.
    <br> While checking Product Name column Some Products start with small letter.
    <br> Transform --> ABC Format -->Capitalize Each Word.
  <br> • Identify any typos present in the "Category" column.
  <br> while Checking Category column There have spelling Mistakes. 'Electronics' is incorrectly written as'Electroni'.
  <br> • Use the find and replace function to standardize the text formats in the "Product Name" column and fix any typos or misspellings in the "Category" column.
   <br>The typos are corrected using Find and replace.select all go to home tab-->Find select-->Find what -->Electroni -->replace with : Electronics -->Replace.
   <br> Like this the Category column based on Product name  corrected using find and replace function.The Unknown value replaced.
# 3) Removing Duplicates:
   • Identify any duplicate rows within the dataset based on the entirety of each row, and remove them if any.
   <br> Select ctrl+A to select all data ,then click  Data- -> Remove Duplicates . select Product ID and Product Name Then click OK . we got a message 3 duplicate values found and removed.
# 4) Splitting and Merging Data:
   • Split the "Product ID" column into two separate columns for " Manufacturing Date" and "Country Code". Remove unnecessary characters, if any.
  <br> Create a column named Product_Updated and add Year by using the following formula.=LEFT([@[Product ID]],6)&"-2026"& "-" &RIGHT([@[Product ID]],2).
   Create 2 columns named Manufacturing Date and Country Code. Entering values to Manufacturing Date through this formula  =LEFT([@[Product_Updated]],11).
   Entering values to Country Code  through this formula =RIGHT([@[Product_Updated]],2).
  <br> • Merge the "Brand Name" and "Product Name" columns into one column named "Product Brand".
   <br>Create new column named Product Brand and apply =[@[Product Name]]&" "&[@[Brand Name]] this formula for concatination.
   # 5) Number Formatting:
   • Format the data type of the "Price" column to currency format. 
   <br>Select Price column-->Home -->Number Format -->Currency.
  <br> • Format the "Manufacturing Date" column to display dates in the "DD-MM-YYYY " format. 
   <br>Select Manufacturing Date--> Home-->Number Format-->Date
  # 6) Conditional Formatting:
   • Apply data bar or color scales conditional formatting in the "Price" column.
   <br>Select Price column--> Home -->Conditional Formatting -->Color Scales.
  <br> • Create a custom rule for conditional formatting in the "Category" column to highlight cells where the category is "Electronics."
    <br>Select Category Column-->Home-->Conditional Formatting-->New Rule-->Select Format only cells that contain-->Edit with rule description-->
    Cell Value-->Specific Text-->Containing-->Electronics-->Format option-->Select color you want--> Click OK --> OK .
   
   
