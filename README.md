# CitiBike Usage Statistics

## Citibike Userbase Summary
Doing some brief analysis of bike usage of Citibike, we are able to come up with the follwing conclusions.
Citibike peak lending hours are around 8am and 5/6 pm on weekdays and the average use of a bike is about 5 hours. Additionally, we have more than twice as many subscribers that are male. They are also nearly 9 times as likely to be a subscriber than use the service for each rental. 
![Userbase](https://github.com/NannGitUser/BikeSharing/blob/main/Our%20Userbase.PNG)

## Rental Duration
Our users vary amount of time they rent the bike. Most users rent the bike 3 to 9 hours with 5 hour rentals being the norm. This applies accross the board, regardless of gender. 
![Checkout Times of Users](https://github.com/NannGitUser/BikeSharing/blob/main/Checkout%20Times%20for%20Users.PNG)
![Checkout Times by Gender](https://github.com/NannGitUser/BikeSharing/blob/main/Checkout%20Times%20by%20Gender.PNG)

## Peak Rental Times
As expected, we peak times for bike rentals in NYC come around 8am and 5pm on weekdays, with an outlier on Saturday at 11am for weekend excursions. This trend appears to be gender neutral as we see the same trends regardless of whether the users registered as Male, Female, or left blank. 
![Trips by Weekday and hour](https://github.com/NannGitUser/BikeSharing/blob/main/Trips%20Workday%20per%20Hour.PNG)
![Trips by Gender (Weekday and Hour)](https://github.com/NannGitUser/BikeSharing/blob/main/Trips%20by%20Gender%20(Weekday%20per%20Hour).PNG)

## Likelihood of Subscription
Males are far more likely to be a subscriber. Looking at statistics, they are nearly 9 times as likely to be a subscriber versus a per-use-renter. 
![Gender and Usertype](https://github.com/NannGitUser/BikeSharing/blob/main/User%20Trips%20by%20Gender%20by%20Weekday.PNG)

## Additional Data
The data provided is limited and does not answer key questions of maintenance. We would like to know where the bikes are idle at any point in time. Citibike data provides endtimes and locations. What we can do is create a blank data sheet with all the location numbers. We would then merge it with the Citibike Data to create multiple entries for each location number. We would then create two calculated fields for the time minus the last time it was dropped off and the difference between that time and the time that it was last checked out. Add a MIN function for each location and field. Then add a If/Then function to determine that it was last dropped off at that time at that location. We then do a count function to determine how many bikes are on each location at the specified time. Additionally, we can figure out how long the bike has been idle at each location with this new table. A much simpler graphic that might be of use would be to look at peak checkout locations at each time to determine where more bikes should be located and at what time. 

Below is a Tableau Link to the data for further Analysis. If you have any questions, or would like to drill down into the information further, please let me know. 
[Tableau link](https://public.tableau.com/views/Module14Challenge_16031112140780/CheckoutTimesforUsers?:language=en&:display_count=y&:origin=viz_share_link)
