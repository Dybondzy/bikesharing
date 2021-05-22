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

Download the NYC Citibank starter code. (Links to an external site.)

Before You Start
In Deliverable 1, you’ll use Pandas to change the datatype of the "tripduration" column from an integer to a datetime datatype to get the time in hours and minutes. Using Tableau instead of Pandas to change the datatype of the "tripduration" column to a "Date and Time" will not produce the same visualizations in Deliverable 2. Trying to change the datatype by creating a calculated field may take more time for the less experienced Tableau user than the steps in Deliverable 1.

Once you change the datatype, you’ll export the DataFrame as a CSV file to use for the visualizations in Deliverable 2. If you export the new CSV file into the same Tableau workbook you used in this module, the "Average Trip Duration" and "Bike Utilization" graphs will be greyed out, and you won’t be able to use them because the datatype for the "tripduration" column has changed. Therefore, we recommend creating a new Tableau workbook to create the visualizations in Deliverable 2, and then you’ll have to recreate the two visualizations from the module in this new Tableau workbook that you’ll use for the Story in Deliverable 3. If you'd like to use the "Bike Utilization" graph in your Story for Deliverable 3, then we suggest creating a new column that contains the converted datatype of the "tripduration" column in Deliverable 1.

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

HINT
NOTE
You can create a new column that contains the conversion if you don't want to change the "tripduration" column to a datetime datatype.

In Step 4, check the datatypes of the DataFrame.
Confirm that the converted values in the "tripduration" column match the following image:
The conversion of the trip duration column to a datetime object.

If you’d like more information on the meaning of the timestamp in the "tripduration" column, read the Deep Dive below:

DEEP DIVE
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
REWIN
