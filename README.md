# Excel-DataCleaning-Dashboard-Insight

# Excel Process Logs

1. [Open the datasets](datasets/data/raw_data/Bike_Buyers_Raw.xlsx)  

2. Create Working Sheet , Pivot Table, Dashboard sheet  

---

## Working Sheet

1. Copy raw data into Working Sheet  
   ![Copy raw data](assets/images/1.Raw data to Worksheet.png)

2. Data overview with filter  
   ![Data overview filter](images/data_overview_filter.png)

3. Remove duplicate from table  
   ![Remove duplicates](images/remove_duplicates.png)

4. Spelling out abbreviation  
   ![Spelling out abbreviation](images/spell_out_abbreviation.png)

5. Make age bracket based on age column  
   ```excel
   =IF(L2<31,"Adolescent","Invalid")
   =IF(L2>=31,"Middle Age",IF(L2<31,"Adolescent","Invalid"))
   =IF(L2>54,"Old",IF(L2>31,"Middle Age",IF(L2<31,"Adolescent","Invalid")))
   ```
   [Age bracket](images/age_bracket.png)

---

## Pivot Table

1. Create Pivot table from working sheet  
   ![Pivot table creation](images/create_pivot_table.png)

2. Put average income as values, gender as rows, purchased bike as column and create clustered column chart with it  
   ![Clustered column chart](images/avg_income_gender_bike.png)

3. Put count of purchased bike as values, commute distance as rows, purchased bike as column and create line chart with it  
   ![Line chart commute distance](images/commute_distance_bike.png)

4. Put count of purchased bike as values, age bracket as rows, purchased bike as column and create line chart with it  
   ![Line chart age bracket](images/age_bracket_bike.png)

5. Copy chart to dashboard sheet  
   ![Copy chart to dashboard](images/copy_chart_dashboard.png)

---

## Dashboard

- Create title, arrange dashboard, create slicer and connect them to pivotchart and add insight  
  ![Dashboard final](images/dashboard_final.png)

