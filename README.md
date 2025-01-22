# eco-driving


## INTRODUCTION
A. Driving Safety and Sustainable Transport
Driving is a common and hazardous activity that is a prominent cause of death worldwide. Driver behavior represents a predominant cause, contributing to over 90% of crashes. Drivers adapt and drive safely in a broad range of situations but fail when expectations are violated or when feedback is inadequate. 
Relatedly, eco-driving is a style of vehicle driving that reduces energy consumption, maximizing mileage per unit of energy consumed. Eco-driving requires adherence to speed limits, accelerating and braking smoothly, avoiding acceleration, use of engine braking, and maintaining a constant speed. Eco-driving may also include vehicle maintenance, trip planning, switching to other transport where appropriate and vehicle choice. Eco-driving may save up to 25% of fuel. There is an overlap between eco-driving and safe driving since safe driving entails observing speed limits and avoiding harsh acceleration and braking.

B. Journey towards a “Car-Light Singapore” 
The recently released Urban Redevelopment Authority (URA) Draft Master Plan 2013 may be a developmental blueprint, but it is also very much a land transport road map - one which supplements the Land Transport Authority's own master plan.
It contains a strong two-pronged theme: reclaiming the city from the car and reducing the need to commute.
- The Straits Times, Nov 28, 2013 https://www.straitstimes.com/singapore/journey-towards-a-car-light-singapore

## DATA DESCRIPTIONS
Dataset extracted from a local car rental company. The dataset consists of multiple tables. Specifically,
1.	CustomerTBL
This table contains data about a customer.
[customerID] uniquely identifies each record

[name] presents the first 4 characters of the customer’s full name. The remaining characters are removed to anonymize the records

[gender] 0 indicates female, 1 indicates male

[member_since] contains the “month day, year” value

[driving_age_yr] contains the customer’s years of driving experience

[postal] contains the first 2 numbers of the customer’s home postal code

3.	VehicleTBL
This table contains data specific to each rental vehicle.
[vehicleID] uniquely identifies each record

[type] contains the value representing a carType

[brand] contains the brand name of the vehicle

[model] contains the model value of the vehicle

[age] is the age (in years) of the vehicle

[total_distance_km] is the vehicle’s total traveled mileage in km.

[full_tank_gal] is the full-tank volume in gallons

[km_per_gal_highway] is the estimated fuel efficiency on the highway

[km_per_gal_city] is the estimated fuel efficiency in the city

[CO2avg_WLTP] is the estimated carbon footprint based on the Worldwide harmonized Light vehicles Test Procedures, i.e., grams of carbon emissions per km

[CO2avg_NEDC] is the estimated carbon footprint based on the New European Driving Cycle, i.e., grams of carbon emissions per km

[fee_per_hour] is the rental fee for an hour of usage

5.	orderTBL
This table contains data specific to an order (i.e., a rental).
[orderID] uniquely identifies each record

[custeromID] represents the customer for the order

[vehicleID] represents the vehicle used in the order

[startDate] represents the starting date of the order

[endDate] represents the ending date of the order

[startTime_hr] represents the time (the specific hour) at which the order commences

[startTime_min] represents the time (the specific minute) at which the order commences

[startTime_ss] represents the time (the specific second) at which the order commences

[endTime_hr] represents the time (the specific hour) at which the order completes

[endTime_min] represents the time (the specific minute) at which the order completes

[endTime_ss] represents the time (the specific second) at which the order completes

[startLoc] contains the first 2 digits of the starting location postal code

[endLoc] contains the first 2 digits of the ending location postal code

[start_fuel_gal] indicates the amount of fuel (in gallons) at the beginning of the order

[end_fuel_gal] indicates the amount of fuel (in gallons) at the end of the order

7.	complaintTBL
This table contains data specific to a complaint.
[complaintID] uniquely identifies each record

[customerID] represents the customer for the complaint

[date] represents the date at which the complaint is filed

[issue] contains the issue category

[severity] contains a numeric severity, i.e., 1 indicates least severe, 5 indicates most severe

[resolved] contains 0 or 1, i.e., 0 indicates unresolved, 1 indicates resolved

9.	incidentTBL
This table contains data about an incident (i.e., violations of traffic regulations)
[incidentID] uniquely identifies each record
[vehicleID] represents the vehicle involved in the incident

[date] indicates the incident date 
[issue] contains an incidentType value

11.	incidentTypeTBL
This table contains data about the 13 types of incidents.

[incidentTypeID] uniquely identifies each record

[detail] provides details on the violation

13.	vehicleTypeTBL
This table contains data about the types of rental vehicles.

[vehicleTypeID] uniquely identifies each record

[type] provides details on the specific type

15.	postalCodeTBL
This table contains the general locations based on the first 2 digits of postal codes.

[postalCode] uniquely identifies each record

[generalLoc] provides the details of the location

 ## Project Structure

 
📂 Project Root  
├── IA.sql                      # SQL queries used for data extraction  
├── IA_db.sql                   # SQL dataset used for the project  
├── README.md                   # Project documentation (this file)  
├── eco-driving query.docx      # Answers to tasks  



 
