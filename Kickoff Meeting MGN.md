Kickoff Meeting MGN 2

**Schedule:**

1. Overview  
2. Mohamed presenting what we think MGN needs (mainly from the initial meeting from september with David, Noah and Damian)  
3. MGN giving us their feedback and overview  
4. What MGN can share with Arvo?  
5. Arvo asking MGN questions  
6. Review of the SOW.  
7. GANTT Chart, RACI and RAID  
8. Done & Acceptance and User Stories

**Our description of MGN’s situation:**

MGN works with logistics companies that have to ship various packages for their clients. MGN has to optimize the following: Whether MGN should ship the package(s) using a carrier (Estes, FedEX, etc.) or if it should instead rent a truck and ship the package(s) potentially making some stops along the way to drop off other packages. MGN must manually calculate the two and decide which one is the most optimal at any given time. 

**Assumptions:** 

1. MGN will always be able to give us the **total** cost associated with renting a truck and using it to ship any given package(s) to different cities (multiple stops).  
   1. As we understand it total cost \= cost of renting the truck \+ cost of delivery (per pallet); cost of delivery \= total cost of lane broken down into cost per mile and then add the cost of making any additional stops (flat fee).  
2. MGN will always be able to give us the **total** cost associated with shipping any given package using a carrier (Estes, FedEX, etc.).  
3. The AI we are building is not a chatbot.

**Questions for MGN:** 

1. Are carriers (Estes, FedEX, etc.) segregated per clients or per shipments? When a client can only use one carrier, does this affect all the clients’ shipments or only a select few that must be shipped through the specifically mentioned carriers.

2. Can you \- and do you usually \- do a mix of shipping with a rented truck and using carriers for the same client? Let’s say that for example a client has 27 palettes all going to one city: You’d use a truck for the 26 palettes and just ship the remaining palette with a carrier?

3. What are all the possible limitations? eg: a truck driver can’t make more than 4/5/7 stops… 

4. How many stops do we max out at? (number of cities a truck driver must go through)  
   1. Could this be a feature where MGN would decide what is the maximum number of stops for any given set of packages?  
   2. How many cities in total are you dealing with (both originating and destinations)?


5. Do we only group by client? \[can we ship palettes from different clients in the same truck?\]

6. Can we assume that clients only operate from one city? i.e all their packages will originate from a one and only one city?  
   1. if not: If a client ships from multiple cities, can a truck stop on the way and pick up another shipment?

7. Do we need to provide the exact route (google maps api) or do we have to give the best path given the constraints as a list of cities? What output is expected from the AI model? 

8. Do clients care about time? Is there a limit clients can wait before shipping/receiving their package? 

9. What is the rate at which you receive new packages (one per hour/day)? We want to know whether \- and potentially how much \-  we should wait for new packages to be dispatched so that we can group them with the other packages and potentially make new?

10. How often do we rerun the optimization engine?

11. Would you accept no human intervention?

**Notes:**

