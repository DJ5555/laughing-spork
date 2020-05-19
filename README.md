# laughing-spork
Hazard Models


In this exercise, we will use the logit and cloglog links in the glm( ) function to estimate  discrete Hazard models. The data file is “HHonors_booking.csv” on Canvas. For 400 Hilton HHonors members, we have the following variables:

customer ID:	The ID of the customer
Booking:	 Whether the customer books a Hilton hotel room in that week{1 = Yes, 0 = No}
Week:	A weekly time period indicator 
Price:	The average price of hotel rooms in that week
Promotion:	Whether a promotion email is send to the customer in that week {1 = Yes, 0 = No}
Income:	The income level of the customer
Gender:	Gender indicator {1 = Male, 0 = Female}

The exercise it to study the effects of time, price and promotion on the hazard of booking a hotel room for each customer. The model also controls for the customer's demographics including income and gender. The hazard of booking a hotel is considered to be "renewed" after a customer books a hotel; i.e., the baseline hazard λ0(t) is reset the λ0(t+1)= λ0(1) if  the customer books a hotel in period (week) t.   
