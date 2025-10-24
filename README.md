# Lyft's Drivers' Lifetime Value
This project analyzes the total value of a driver to Lyft over the entire projected lifetime of a driver.

After exploring and analyzing the data, we can answer:

1.  Recommend a Driver's Lifetime Value (i.e., the value of a driver to Lyft over the entire projected lifetime of a driver).
    
2.  Please answer the following questions:
    
    *   What are the main factors that affect a driver's lifetime value?
        
    *   What is the average projected lifetime of a driver? That is, once a driver is onboarded, how long do they typically continue driving with Lyft?
        
    *   Do all drivers act alike? Are there specific segments of drivers that generate more value for Lyft than the average driver?
        
    *   What actionable recommendations are there for the business?
        
3.  Prepare and submit a writeup of your findings for consumption by a cross-functional audience.
    

You can make the following assumptions about the Lyft rate card:

*   Base Fare $2.00
    
*   Cost per Mile $1.15
    
*   Cost per Minute $0.22
    
*   Service Fee $1.75
    
*   Minimum Fare $5.00
    
*   Maximum Fare $400.00
    

Data Description
----------------

You'll find three CSV files attached with the following data:

**driver\_ids.csv**

*   **driver\_id** Unique identifier for a driver
    
*   **driver\_onboard\_date** Date on which driver was on-boarded
    

**ride\_ids.csv**

*   **driver\_id** Unique identifier for a driver
    
*   **ride\_id** Unique identifier for a ride that was completed by the driver
    
*   **ride\_distance** Ride distance in meters
    
*   **ride\_duration** Ride duration in seconds
    
*   **ride\_prime\_time** Prime Time applied on the ride
    

**ride\_timestamps.csv**

*   **ride\_id** Unique identifier for a ride
    
*   **event** describes the type of event; this variable takes the following values:
    
    *   _requested\_at_ - passenger requested a ride
        
    *   _accepted\_at_ - driver accepted a passenger request
        
    *   _arrived\_at_ - driver arrived at pickup point
        
    *   _picked\_up\_at_ - driver picked up the passenger
        
    *   _dropped\_off\_at_ - driver dropped off a passenger at destination
        
*   **timestamp** Time of event
    

You can assume that:

*   All rides in the data set occurred in San Francisco
    
*   All timestamps in the data set are in UTC
