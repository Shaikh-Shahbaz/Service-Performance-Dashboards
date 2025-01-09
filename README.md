# Service-Performance-Dashboards
## Step 1 - Preparing the data for the dashboard :

  1. Using Tableau prep to clean the data and add additional fields.
  2. Check if the date fields have the date data type.
  3. Create additional fields for both the start date and end date. Fields like year, quarter, month, and year-quarter would be useful in the analysis.
  4. The field service division owner had a couple of values (Municipal Licensing & Standards, Parks, Forestry & Recreation) with the string “&” in one value and “and” in 
     another. Cleaned them by renaming the value with “and” to “&”.
  5. Use ChatGPT to get additional details for each of the wards. Information like ward name, latitude, and longitude will help visualize the data using maps.
     Prompted ChatGPT to generate a table with the data for all the wards in the city of Toronto by referring to the city of Toronto website and asked it to add additional 
     details like ward name, latitude,and longitude. This data should add further context and enable the use of maps for data visualization.
     Resources - 
      I .https://www.toronto.ca/city-government/data-research-maps/neighbourhoods-communities/ward-profiles/
      II .https://www.kaggle.com/datasets/sidharth178/toronto-neighborhood-data?utm_source=chatgpt.com
  
     Joining these two datasets in tableau prep. I have used a LEFT join with the Test data shared by city of Toronto as the left table and joined it with the ward_details 
     table which has every ward’s information like the ward_name, latitude and longitude. I am using the ward_id from the test data and the ward number from the ward_details 
     table as the key to join these datasets.

        <img width="630" alt="Tableau Prep Flow" src="https://github.com/user-attachments/assets/b94fb511-7924-4bab-b3ed-844dee1fbbad" />

     ## Metadata -
        ![image](https://github.com/user-attachments/assets/56745122-d67a-4b3f-a90c-41122202b889)
     

