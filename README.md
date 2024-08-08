# Pizza sales Analytics Dashboard


## Problem Statement

This dashboard helps the Pizza chain owner team to understand the distribution of pizza sales . It helps the management team to 
developed and choose better places to choose their pizza chian hop.Helps to  give insights regarding the daily,hourly sales of pizzas based on different paramaeters like location,time  .Calculated charts will give a clear idea about the pizza category which is most popular and other details which will help to improve business



### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a xlsx file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : 
 

### Data model 

![image](https://github.com/9475Abhinaba/Revenue-insights-in-hospitality-management-domain/assets/169307645/0f61dd0d-3836-493b-be0a-01e2fa546d13)

        
- Step 8 : New measure was created for total orders

Following DAX expression was written for the same,
        
     total_orders = DISTINCTCOUNT('order_details_lookup_prac'[order_id])
	 


 
![image](https://github.com/9475Abhinaba/Revenue-insights-in-hospitality-management-domain/assets/169307645/fc695083-126f-4ab8-abee-ba63b5e179dd)

        
 - Step 9 : New measure was created to get total pizza sold,
 
 Following DAX expression was written for the same,

![image](https://github.com/9475Abhinaba/Revenue-insights-in-hospitality-management-domain/assets/169307645/5f37e36c-d1ff-4212-b16b-984a9cb9623a)

 
 - Step 10 : New measure was created to calculate total sales
 
 Following DAX expression was written for the same,
 
        Total Revenue = SUMX('Merge1','Merge1'[pizzas.price]*'Merge1'[quantity])
 
 
![image](https://github.com/9475Abhinaba/Revenue-insights-in-hospitality-management-domain/assets/169307645/10e6d167-1eec-4d16-8922-29a2fd8ad267)


# Insights

A  report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;


### [1] trend of monthly pizza sales,hourly pizza sales
  ![image](https://github.com/9475Abhinaba/Revenue-insights-in-hospitality-management-domain/assets/169307645/a164e74f-35a3-43b2-9b68-8ef228233ba6)

### [2] Pizza slaes bassed on categoty ,size 
![image](https://github.com/9475Abhinaba/Revenue-insights-in-hospitality-management-domain/assets/169307645/e0798107-f72e-4f8f-9d0b-07b8c5c6f5f5)

### [3] Top five ,Bottom five pizzas sold
![image](https://github.com/9475Abhinaba/Revenue-insights-in-hospitality-management-domain/assets/169307645/5d546c3e-b017-493c-8b89-a5b776f5168d)
### [4] Heatmap for hourly daily sales 
![image](https://github.com/9475Abhinaba/Revenue-insights-in-hospitality-management-domain/assets/169307645/81c5403d-df6c-4497-ab72-f629db2dcf78)
