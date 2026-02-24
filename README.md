# Excel-DataCleaning-Dashboard-Insight

# Excel Process Logs

1. [Open the datasets](datasets/data/raw_data/Bike_Buyers_Raw.xlsx)  

2. Create Working Sheet , Pivot Table, Dashboard sheet  

---

## Working Sheet

1. Copy raw data into Working Sheet  
   ![Copy raw data](assets/images/1.Raw_data_to_Worksheet.png)

2. Data overview with filter  
   ![Data overview filter](assets/images/2.Data_overview_with_Filter.png)

3. Remove duplicate from table  
   ![Remove duplicates](assets/images/3.Remove_duplicate.png)

4. Spelling out abbreviation  
   ![Spelling out abbreviation](assets/images/4.Spelling_out_Abbreviation.png)

5. Make age bracket based on age column  
   ```excel
   =IF(L2<31,"Adolescent","Invalid")
   =IF(L2>=31,"Middle Age",IF(L2<31,"Adolescent","Invalid"))
   =IF(L2>54,"Old",IF(L2>31,"Middle Age",IF(L2<31,"Adolescent","Invalid")))
   ```
   [Age bracket](assets/images/5.New_field_AgeBracket.png)

---

## Pivot Table

1. Create Pivot table from working sheet  
   ![Pivot table creation](assets/images/6.Create_pivot_table_from_worksheet.png)

2. Put average income as values, gender as rows, purchased bike as column and create clustered column chart with it  
   ![Clustered column chart](assets/images/7.Clustered_column_chart_gender.png)

3. Put count of purchased bike as values, commute distance as rows, purchased bike as column and create line chart with it  
   ![Line chart commute distance](assets/images/8.Line_chart_commute_distance.png)

4. Put count of purchased bike as values, age bracket as rows, purchased bike as column and create line chart with it  
   ![Line chart age bracket](assets/images/9.Line_chart_age_bracket.png)

5. Copy chart to dashboard sheet  
   ![Copy chart to dashboard](assets/images/10.Copy_chart_to_dashboard_sheet.png)

---

## Dashboard

- Create title, arrange dashboard, create slicer and connect them to pivotchart and add insight  
  ![Dashboard final](assets/images/11.Dashboard_slicer_insight.png)

