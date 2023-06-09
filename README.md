# Capston-Project1-Python-Module
# Objective:
Provided with a hotel bookings dataset.The main objective is perform EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other.

# Dataset:
This dataset contains booking information for a city hotel and a resort hotel. It contains the following features.

- hotel: Name of hotel ( City or Resort)
- is_canceled: Whether the booking is canceled or not (0 for no canceled and 1 for canceled)
- lead_time: time (in days) between booking transaction and actual arrival.
- arrival_date_year: Year of arrival
- arrival_date_month: month of arrival
- arrival_date_week_number: week number of arrival date.
- arrival_date_day_of_month: Day of month of arrival date
- stays_in_weekend_nights: No. of weekend nights spent in a hotel
- stays_in_week_nights: No. of weeknights spent in a hotel
- adults: No. of adults in single booking record.
- children: No. of children in single booking record.
- babies: No. of babies in single booking record. 
- meal: Type of meal chosen 
- country: Country of origin of customers (as mentioned by them)
- market_segment: What segment via booking was made and for what purpose.
- distribution_channel: Via which medium booking was made.
- is_repeated_guest: Whether the customer has made any booking before(0 for No and 1 for 
                     Yes)
- previous_cancellations: No. of previous canceled bookings.
- previous_bookings_not_canceled: No. of previous non-canceled bookings.
- reserved_room_type: Room type reserved by a customer.
- assigned_room_type: Room type assigned to the customer.
- booking_changes: No. of booking changes done by customers
- deposit_type: Type of deposit at the time of making a booking (No deposit/ Refundable/ No refund)
- agent: Id of agent for booking
- company: Id of the company making a booking
- days_in_waiting_list: No. of days on waiting list.
- customer_type: Type of customer(Transient, Group, etc.)
- adr: Average Daily rate.
- required_car_parking_spaces: No. of car parking asked in booking
- total_of_special_requests: total no. of special request.
- reservation_status: Whether a customer has checked out or canceled,or not showed 
- reservation_status_date: Date of making reservation status.

Total number of rows in data: 119390
Total number of columns: 32

Data Cleaning and Feature Engineering
(1) Removing Duplicate rows-
All duplicate rows were dropped.

(2) Handling null values-
Null values replaced with zeros.

(3) Creating new columns-
Created new column total_stay by adding stays_in_weekend_nights+stays_in_week_nights.

# Exploratory Data Analysis:
Performed EDA and tried answering the following questions:
```

 Q1)which country has maximun visitrs?
 Q2)which market segment has high visitors?
 Q3)which distribution channel gets hights bookings?
 Q4)get to know are the guests visited again?
 Q5)get to know how many guest had canceled booking previously?
 Q6)which rooms types are highly demanded by the guests?
 Q7)how many guests have changes the booking?
 Q8)how many customer booked hotel through deposits?
 Q9)which agents have highest no of bookings?
 Q10)what type of customer visited the hotel?
 Q11)how many customers demanded for a car parking spaces?
 Q12) how many customers generaly do special requests?
 Q13) which months are the busiests months?
 Q14)create a new variable total_stay?
 Q15)number of days guests prefer to stay?
 Q16)what type of meal preferd most by the guests?
 Q17)which type of hotel has hights cancelations?
 Q18)which hotel has the highest arrival guest?
 Q19)what are the average lead times for hotels?
 Q20)in which hotel guests prefer to stay longer?
 Q21)for weekend nights which hotel prefer more?
 Q22)for week nights which hotel prefer more?
 Q23)what type of market segment prefer which hotel more?
 Q24)which hotel has high waiting time?
 Q25)which month has high adr value?
 Q26)what type of customer have special request?
 Q27)find the monthly  canceltions for each hotel?
 Q28)find the monthly avg adr for each hotel?
 Q29)find monthly average lead time for each hotel?
```
# Graphs and Charts used for data visualization:
Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:
-Bar Plot.
-Histogram.
-Pie Chart.
-Line Plot.
-Kde plot.
-Box Plot.
-Count Plot.

# Insigts found :
```
1)the top countries which vistited most to this hotels are'PRT','GBR','FRA','ESP','DEU','ITA','IRL','BEL','BRA','NLT.
2)more than 50% of the booking takes place place through Online TA(Tralaval Agent) and offline TA.
3)online TA has the high percentage of the arriving to the hotel (more then 50%)
4)repeated guests are very less to this hotel(both city hotel and resort). which is less than 1%.that means if any coustomer visit to this hotel there are high chances that customer will be new one.
5)large number of guests are prefer A type of room.
6)also guest who come to visit this hotels has very low record of booking changes.
7)more than 90% of the customer pre no-deposit type of bookings.
8)in this hotel transient type of customers are visit most.
9)more than 90% of the customers does not need parking spaces , very less number of customers required 1 or more parking spaces
10)more than 50% customers dont do any special request.
11)in this dataframe i found that March to August are the bussiest month of the years.
12)more than 50% of the customers prefer BB(bed and breakfast) type of meal.
13)City Hotel type of hotel has both high cancelation and arrival rate of the customers.
14)customers generally prefer Resot type of hotel to stay longer due to that Resort type of hotel has high lead time then city type of hotel.
15)due to high business of city type hotel this hotels have high waiting time as compaird to resort type of hotels.
16)as we can see in august month has both booking cancelation rate and customer arrival rate.
17)as we can see adr valuses for city hotels are much higher than the resort hotels.
18)also for resort hotels 'January' ,'February','March','October','November','December' are the lowest adr months.
19)generally for city hotels adr rates are not as low as resort hotel but ascompair to other months 'January','February','March'and 'November','December' are lower adr rate months for city hotels.
20)'July' and 'August' are the highest adr rate value for resort hotel than city hotel.
21)'May','June','Jully','August','September','October' are the highest lead time month for the both city type and resort type hotel.but resort type hotel has high lead time than city type hotel.
```
# conclusions:
```
1)county base should be diversified.
2)In the month of July and August has high arrival rate and cancelations rate also.
3)adr value per room goes on increse from may till the september and then goes on decresing.
4)for the longer stay customers generally prfer to resort hotels than the city hotels.
5)repetaion rate of customers is very low.
6)city hotels are busiest hotels than resort hotels.
7)large numbers of customers arrivels through online TA/TO.
8)Also large no of cancelation happned those who have done booking through online TA/TO.
```
