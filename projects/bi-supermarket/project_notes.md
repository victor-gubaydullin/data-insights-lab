## Business Setting

Within our project, we imagine that an Azerbaijani supermarket chain was acquired by a European chain that has an "English-first" standard and now requires proper reporting for their newly hired **Category Manager** and **Sales Lead**. We, as BI data analysts, now have the honor to provide the new stakeholders with insights and implement certain reporting for these new branches. Luckily, they will already be fine with Excel-based reports and some auto-generated PDF slides.

## Our observations

The data we initially received (and we assume that we will continue to receive this kind of data from time to time) is sourced from 20 different branches of an Azerbaijani supermarket and therefore has some local specifics, e.g., the language.

## Our approach

To fulfill that goal, we first need a proper data pipeline. The new branches are delivering .csv data to us, but we must ensure that our data will from now on be properly stored within a SQL database.

Therefore, here are our todos:
1) Establish a MySQL database.
    - Write a models.py module with table(s) definitions and relations (if needed).
        - Ensure our table will have all the necessary dimensions and measures and in the correct format.
    - Write a data_utils.py module with utility functions for us to operate with our database from Python.
2) Establish a data pipeline that will process our data into the database.
    - Read .csv data.
    - Translate it.
        - No use of API due to DSGVO, simple pre-defined dictionaries and a pop-up if a value is not found.
    - Transform it (if needed).
3) 
