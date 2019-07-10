# mtn_work :
Loaded variables into the workbook.Variables 'df' represents the cells_geo dataset. Variable df1,df2,df3 represens the three Moringa datasets respectively
# cleaning : 
Changed the individual column names to lower case using the syntax 'changing columns of dataset 1 to lower case'.
Grouped the df1,df2,df3 datasets using concat function.  dataframe = pd.concat([df1_merged, df2_merged, df3_merged], ignore_index=False)
Dropped all unecessary columns(for the analysis) from the merged dataset
Splitted date and time
# Final Work
Finding the cities with the most product usage. dataframe.groupby(['date', 'villes']).size()
Fining cities that had most product usage within business hours. business_hours.groupby('villes')['villes'].count().sort_values(ascending = False)
Fining cities that had most product usage within business hours. home_hours.groupby('villes')['villes'].count().sort_values(ascending = False)
Computed the region and area with the most product usage
Finding cities that used the product most. dataframe.groupby('villes')['villes'].count().sort_values(ascending = False).head()


 
