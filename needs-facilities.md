# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given there is a mechanism to count visitors per day from sensor data and 
  store the day wise information in cloud/ or in database
  
  When the week ends
  
  Then a report is generated with number of visitors against the days
  for that week.

Scenario: Alert when seating capacity is full

  Given there is a mechanism to count visitors at any given time 
  from sensor data

  When the number of visitors cross the 70 percent of the 
  capacity of hospital

  Then an alert trigger is sent to the facilities manager.
