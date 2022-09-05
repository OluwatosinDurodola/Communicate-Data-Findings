# No Show Appointment Data Exploration
## by Oluwatosin Durodola


## Dataset

This dataset consist of over 110,000 medical appointments collected in Brazil and is focused on the question of whether or not patients show up for their appointment. A number of characteristics about the patient are included in each row including age, gender and other patients info. The dataset and info with the 14 feature documentation available [here](https://www.google.com/url?q=https://www.kaggle.com/joniarroba/noshowappointments&sa=D&source=editors&ust=1653562576691069&usg=AOvVaw1NcnXiqZwomcljy7DxTZWW)

Additional fea 3 features was included by me i.e. waiting days, appointment_day, and
age_group. Six data points were removed from the analysis due to inconsistencies or
missing information.


## Summary of Findings

In the exploration, there are about 80% (88,207) out of over 110,521 patients
who showed up for their appointment while the remaining 20% (22,314) didn't. 
I found that there was a strong relationship between the difference of schedule date
to appointment date of a patient and his/her response to show and no show appointment,
with a new column being created from schedule date and appointment date to get
waiting days of each patients. 0 to 2 Waiting days taken large values of frequency
while 179 being the highest waiting days has the lowest frequency.

The relationship between the waiting days and no show shows that the longer the
waiting days, the more are they discouraged. There is also a positive correlation
between age and waiting days, and noticed that the higher the age and waiting
days the lower the patients frequency.


## Key Insights for Presentation

For the presentation, I focus on just the influence of the waiting days and age
on patients no show and leave out most of the intermediate derivations.
I start by introducing the distribution of no_show variable then waiting days and
age variable, then plot the heatmap of waiting days vs age.

Afterwards, I introduce waiting days variables by no_show variable using the
box plots of waiting days across no_show since it's the clearest example of
why the patients are not showing up for appointment. I further included the
no_show to it with hue in the bar plot to see if there is any bias but it shows
the same return without a bias.