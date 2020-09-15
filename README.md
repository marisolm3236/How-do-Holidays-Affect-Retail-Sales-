# How-do-Holidays-Affect-Retail-Sales-
Our overall goal for this project is to explore the relationship between the columns IsHoliday and Weekly_Sales. Moreover, we were interested in seeing how Store, Dept, Type, Temperature, Fuel_Price, CPI, and Unemployment separately affected this relationship. We wanted to ask questions such as, "What will weekly sales look like if it's a holiday or not a holiday for each store or department?" We aimed to look for any trends and correlations between sales and holidays, and between sales and holidays given a third variable.
We had three data sets: Store, Store features and Sales. We used `pd.merge()` to merge df_sales and df_store_feat. We did this using a left join to produce a complete set of records from df_sales, with the matching records (where available) in df_store_feat. We merged on the three columns listed below because we wanted matching records based on date, store, and whether or not it was a holiday. This is because we wanted to keep all 'Weekly_Sales` information because that is what we are analyzing.

The holidays are named October 9, November 26, December 2, and December 31. Which does not match with the actual dates for Super Bowl, Labor Day, Thanksgiving, Black Friday and Christmas

Because questioned the validity of these holidays (the only holiday for the week of October 9 is Leif Erikson Day, which doesn't make any sense while Christmas week isn't considered a holiday). We wanted to create a new column called `IsHoliday_4` consisting of four major holidays:
- Super Bowl (February 7, 2010) week
- Labor Day (September 6, 2010) week
- Thanksgiving/Black Friday (November 26, 2010) week
- Christmas (December 25, 2010) week

We then individually analyzed Super Bowl, Labor Day, Thanksgiving, Black Friday and Christmas.

While we did see that there were peaks in sales corresponding to certain holidays, we wanted to explore this further than plotting IsHoliday and Weekly Sales. We saw that type C had the smallest difference between weekly sales during holidays and non holidays while types a and b had bigger differences. We saw that unemployent, CPI, fuel price, and temperature had little effect on weekly sales based on whether or not it was a holiday. Moreover, we saw variation in weekly sales based on departments and stores in some cases. 
