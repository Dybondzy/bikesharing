# bikesharing


Module 14

Tableau


Background
Now that we've gotten a good idea of how to create our story, there is still some more work to be done to convince investors that a bike-sharing program in Des Moines is a solid business proposal. To solidify the proposal, one of the key stakeholders would like to see a bike trip analysis.

For this analysis, you’ll use Pandas to change the "tripduration" column from an integer to a datetime datatype. Then, using the converted datatype, you’ll create a set of visualizations to:

Show the length of time that bikes are checked out for all riders and genders
Show the number of bike trips for all riders and genders for each hour of each day of the week
Show the number of bike trips for each type of user and gender for each day of the week.
Finally, you’ll add these new visualizations to the two you created in this module for your final presentation and analysis to pitch to investors.

What You're Creating
This new assignment consists of two technical analysis deliverables and a written report to present your results. You will submit the following:

Deliverable 1: Change Trip Duration to a Datetime Format
Deliverable 2: Create Visualizations for the Trip Analysis
Deliverable 3: Create a Story and Report for the Final Presentation
Files
Use the following link to download the Challenge starter code.

Download the NYC Citibank starter code.
! https://github.com/Dybondzy/bikesharing/blob/main/NYC_CitiBike_Challenge_starter_code.ipynb

Before You Start
In Deliverable 1, you’ll use Pandas to change the datatype of the "tripduration" column from an integer to a datetime datatype to get the time in hours and minutes. Using Tableau instead of Pandas to change the datatype of the "tripduration" column to a "Date and Time" will not produce the same visualizations in Deliverable 2. Trying to change the datatype by creating a calculated field may take more time for the less experienced Tableau user than the steps in Deliverable 1.

Once you change the datatype, you’ll export the DataFrame as a CSV file to use for the visualizations in Deliverable 2. If you export the new CSV file into the same Tableau workbook you used in this module, the "Average Trip Duration" and "Bike Utilization" graphs will be greyed out, and you won’t be able to use them because the datatype for the "tripduration" column has changed. Therefore, we recommend creating a new Tableau workbook to create the visualizations in Deliverable 2, and then you’ll have to recreate the two visualizations from the module in this new Tableau workbook that you’ll use for the Story in Deliverable 3. If you'd like to use the "Bike Utilization" graph in your Story for Deliverable 3, then we suggest creating a new column that contains the converted datatype of the "tripduration" column in Deliverable 1.

! https://github.com/Dybondzy/bikesharing/blob/main/NYC_CitiBike_Challenge.ipynb

Deliverable 1: Change Trip Duration to a Datetime Format (20 points)
Deliverable 1 Instructions
Using Python and Pandas functions, you’ll convert the "tripduration" column from an integer to a datetime datatype to get the time in hours, minutes, and seconds (00:00:00). After you convert the "tripduration" column to a datetime dataytpe, you’ll export the DataFrame as a CSV file to use for the trip analysis in Deliverable 2.

Follow the instructions below to complete Deliverable 1.

Download the NYC_CitiBike_Challenge_starter_code.ipynb file into your bikesharing folder, and rename it NYC_Citibike_Challenge.ipynb.
Use the instructions below to add code where indicated by the numbered-step comments in the starter code file. We have provided the dependencies you will need for this challenge.
In Step 1, create a DataFrame from the 201908-citibike-tripdata.csv file.
In Step 2, check the datatypes of each column in the DataFrame.
In Step 3, convert the "tripduration" column to a datetime datatype by passing the DataFrame column and the units inside the to_datetime() function.
If you’d like a hint on how to convert an integer datatype to a datetime datatype, that’s totally okay. If not, that’s great too. You can always revisit this later if you change your mind.
! https://github.com/Dybondzy/bikesharing/blob/main/NYC_CitiBike_Challenge.ipynb


In Step 4, check the datatypes of the DataFrame.
Confirm that the converted values in the "tripduration" column match the following image:
The conversion of the trip duration column to a datetime object.

In Step 5, export the DataFrame as a new CSV file without the index column. Use this new CSV file for Deliverable 2.
Deliverable 1 Requirements
You will earn a perfect score for Deliverable 1 by completing all requirements below:

The data in the "tripduration" column is converted to a datetime datatype and has the correct time format (15 pt)
The DataFrame is exported as a new file without the index column (5 pt)
Deliverable 2: Create Visualizations for the Trip Analysis (50 points)
Deliverable 2 Instructions
Using Tableau, create visualizations that show:

How long bikes are checked out for all riders and genders.
How many trips are taken by the hour for each day of the week, for all riders and genders.
A breakdown of what days of the week a user might be more likely to check out a bike, by type of user and gender.

Open Tableau and import the new CSV file that contains the conversion of the "tripduration" column to a datetime datatype in a new Tableau workbook.

Follow the instructions below to complete Deliverable 2.

Create the Checkout Times for Users Viz
In this visualization, you’ll graph the length of time that bikes are checked out for all riders.

Add the number of records or the generated field that counts the number of records in the CSV file to the Rows.
Add the "tripduration" column you converted to the Columns, and filter the "More" option by "Hour".
Add the "tripduration" column again to the Columns, and filter the "More" option by "Minute", and then change the values from "discrete" to "continuous".
Add the "tripduration" column that shows the "Hour" to the Filters field, and select "Show Filter".
Edit the X and Y axis labels by right-clicking on the axis label and selecting "Edit Axis".
Your graph should look similar to the following image:
! [link to dashboard](https://public.tableau.com/app/profile/dinah.bondzie/viz/NYC_Citibike_Challenge_Module14/CheckoutTimesforUsers)

Create the Checkout Times by Gender Viz
In this visualization, you’ll graph the length of time that bikes are checked out for each gender.

Repeat steps 1-4 of the "Checkout Times for Users" visualization.
Add the converted column for gender as a color to the Marks field, add it to the Filters field, and select "Show Filter".
Edit the X and Y axis labels by right-clicking on the axis label and selecting "Edit Axis".
Your graph should look similar to the following image:
! [link to dashboard](https://public.tableau.com/app/profile/dinah.bondzie/viz/NYC_Citibike_Challenge_Module14/CheckoutTimesbyGender)

Create the Trips by Weekday for Each Hour Viz
In this visualization, you’ll graph the number of bike trips by weekday for each hour of the day as a heatmap.

Add the "Starttime" column to the Rows, and filter the "More" option by "Hour".
Add the "Stoptime" column to the Columns, and filter the “More” option by "Weekday".
Add the number of records or the generated field that counts the number of records in the CSV file to the Marks field as a color. Select "Automatic" for the type of graph to create the heatmap.
Format the Y axis of the Starttime by Hour to show the 12-hour format
Create the Trips by Weekday for Each Hour Viz
In this visualization, you’ll graph the number of bike trips by weekday for each hour of the day as a heatmap.

Add the "Starttime" column to the Rows, and filter the "More" option by "Hour".
Add the "Stoptime" column to the Columns, and filter the “More” option by "Weekday".
Add the number of records or the generated field that counts the number of records in the CSV file to the Marks field as a color. Select "Automatic" for the type of graph to create the heatmap.
Format the Y axis of the Starttime by Hour to show the 12-hour format
! [link to dashboard](https://public.tableau.com/app/profile/dinah.bondzie/viz/NYC_Citibike_Challenge_Module14/TripsbyWeekdayperHour)

Create the Trips by Gender (Weekday per Hour) Viz
In this visualization, you’ll graph the number of bike trips by gender for each hour of each day of the week as a heatmap.

Repeat steps 1-3 from the "Trips by Weekday per Hour" visualization.
Add the converted column for "Gender" to the Columns and to the Filters field, and select "Show Filter".
Format the Y axis of the Starttime by Hour to show the 12-hour format.
Optional: Format the X axis of Stoptime by Weekday as "Abbreviation".
Your graph should look similar to the following image:
! [link to dashboard](https://public.tableau.com/app/profile/dinah.bondzie/viz/NYC_Citibike_Challenge_Module14/UserTripsbyGenderbyWeekday)

Create the User Trips by Gender by Weekday Viz
In this visualization, you’ll graph the number of bike trips by gender for each hour for each day of the week as a heatmap.

Add the converted column for "Gender" to the Columns and to the Filters field, and select "Show Filter".
Add the "Usertype" to the Rows and to the Filters field, and select "Show Filter".
Add the "Starttime" column to the Rows, and filter the "More" option by "Weekday".
Add the number of records or the generated field that counts the number of records in the CSV file to the Marks field as a color. Select "Automatic" for the type of graph to create the heatmap.
Your graph should look similar to the following image:
! [link to dashboard](https://public.tableau.com/app/profile/dinah.bondzie/viz/NYC_Citibike_Challenge_Module14/UserTripsbyGenderbyWeekday)

Deliverable 2 Requirements
You will earn a perfect score for Deliverable 2 by completing all requirements below:

There is a line graph displaying the number of bikes checked out by duration for all users, and the graph can be filtered by the hour (10 pt)
There is a line graph displaying the number of bikes that are checked out by duration for each gender by the hour, and the graph can be filtered by the hour and gender (10 pt)
A heatmap is created showing the number of bike trips for each hour of each day of the week (10 pt)
A heatmap is created showing the number of bike trips by gender for each hour of each day of the week, and the heatmap can be filtered by gender (10 pt)
A heatmap is created showing the number of bike trips for each type of user and gender for each day of the week, and you can only filter by user and gender (10 pt)
Deliverable 3: Create a Story and Report for the Final Presentation (30 points)
Deliverable 3 Instructions
For this part of the Challenge, you’ll create a story in Tableau and write a report that describes the key outcomes of the NYC Citibike analysis you did in the module and in Deliverable 2.

Follow the instructions below to complete Deliverable 2.

In Tableau, create a new Story using visualizations that will support the key findings you want to show.

You must use the five visualizations that you created in Deliverable 2.
You must use at least two visualizations that you created in this module.
In your README markdown file, include the following:
Overview of the analysis: Explain the purpose of this analysis.
Results: Using the visualizations you have in your Tableau Story, describe the results of each visualization underneath the image.
Summary: Provide a high-level summary of the results and two additional visualizations that you would perform with the given dataset.
Deliverable 3 Requirements
You will earn a perfect score for Deliverable 3 by completing all requirements below:

Structure, Organization, and Formatting (6 points)
The written analysis has the following structure, organization, and formatting:

There is a title, and there are multiple sections. (2 pt)
Each section has a heading and subheading. (2 pt)
Links to images are working and displayed correctly. (2 pt)
Analysis (24 points)
The written analysis has the following:

Overview of the statistical analysis:

The purpose of the analysis is well defined. (5 pt)
Results:

There are at least seven visualizations for the NYC Citibike analysis (7 pt)
There is a description of the results for each visualization (7 pt)
Summary:

There is a high-level summary of the results and two additional visualizations are suggested for future analysis (5 pt)
Submission
Once you’re ready to submit, make sure to check your work against the rubric to ensure you are meeting the requirements for this Challenge one final time. It’s easy to overlook items when you’re in the zone!

As a reminder, the deliverables for this Challenge are as follows:

Deliverable 1: Change Trip Duration to a Datetime Format
Deliverable 2: Create Visualizations for the Trip Analysis
Deliverable 3: Create a Story and Report for the Final Presentation
Upload the following to your bikesharing GitHub pages repository:

The NYC_Citibike_Challenge.ipynb file.
An updated README.md that has your written analysis with visualizations. Also, embed the Tableau Public link in your README.md file. You can do this in a few ways, but here are the two most popular ones:

! [link to dashboard](https://public.tableau.com/app/profile/dinah.bondzie/viz/NYC_Citibike_Challenge_Module14/CheckoutTimesforUsers)

! [link to dashboard](https://public.tableau.com/app/profile/dinah.bondzie/viz/NYC_Citibike_Challenge_Module14/CheckoutTimesbyGender)

! [link to dashboard](https://public.tableau.com/app/profile/dinah.bondzie/viz/NYC_Citibike_Challenge_Module14/TripsbyWeekdayperHour)

! [link to dashboard](https://public.tableau.com/app/profile/dinah.bondzie/viz/NYC_Citibike_Challenge_Module14/UserTripsbyGenderbyWeekday)


