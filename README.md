
# Project: Medical Appointments No Shows Exploration
This dataset collects information from 110k medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment. A number of characteristics about the patient are included in each row such as:

* ‘ScheduledDay’ tells us on what day the patient set up their appointment.
* ‘Neighborhood’ indicates the location of the hospital.
* ‘Scholarship’ indicates whether or not the patient is enrolled in Brasilian welfare program Bolsa Família.
* Possible diseases such as: hypertension, diabetes, alcoholism, handicap
The dependent variable - No-show- says ‘No’ if the patient showed up to their appointment, and ‘Yes’ if they did not show up. (This is later reformated during analysis). The original dataset has been sourced from Kaggle Dataset: Medical Appointment No Shows on 29th October 2018.

## Analysis Goal
To find factors that are important to know in order to predict if a patient will show up for their scheduled appointment

## Tech Stack

**Python:** Pandas, Numpy, Seaborn, Matplotlib

## Analysis Result
**The report text is contained in Markdown cells in the jupyter notebook to clearly distinguish comments and findings from code work.**\
Using both Univariate and Bivariate analysis involving distribution plots using proportions due to the imbalance of the dataset, it could be seen that:

* Age is correlated to Hipertension and  these two variables have effects on whether a patient would show up for appointment or not. The probability of patient showing up increases with age.
* SMS notification for the appointment is quite neccessary for a patient to show up for appointment.
* Scholarship,Diabetes, Alcoholism, Handcap, Waiting_Days, Gender', Neighbourhood and Scheduled_Day_Of_The_Week doesn't seem to affect the decision of a patient in showing up or not.

## Limitations
The presence of invalid entries posed a great limitation to this project. Such situations are explained below:

* It was realized during analysis that some appointments were scheduled for past date, i.e the AppointmentDay came before the ScheduledDay. There could be so many occurences of wrong inputs like that which would have appeared valid when checked and affect the result of the analysis.
* About 1.3K duplicated entries were discovered and removed from the dataset. Removing these entries that came with different AppointmentID and other invalid entries reduced the volume of data used for this analysis and could make the analysis result inaccurate.
Also;

* The imbalance of the dataset which might have resulted from the fact that the data available is only recorded for some occurences in a year also posed a bit of limitation on the analysis result. Having data spanning over different years would have helped in the understanding of the patients better.
* There might be many other factors that can effect individual's decision to show up for appointment or not which are not covered in the dataset. Factors such as the patient's occupation and so many others.

## Screenshots
![Screenshot (92)](https://user-images.githubusercontent.com/58152694/143496861-a5c6d9a0-aceb-4f4a-808e-b8fac5142c79.png)

## Acknowledgements

 - [Udacity](https://udacity.com)
 - [Kaggle-Data Source](https://www.kaggle.com/joniarroba/noshowappointments)

## References
* https://stackoverflow.com/questions/35692781/python-plotting-percentage-in-seaborn-bar-plot
* https://www.geeksforgeeks.org/create-a-stacked-bar-plot-in-matplotlib/
* https://seaborn.pydata.org/generated/seaborn.barplot.html

## Feedback
If you have any feedback, please reach out to me at ayangidel@hotmail.com

