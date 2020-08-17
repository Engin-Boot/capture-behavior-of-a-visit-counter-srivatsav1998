# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given we have unique cards issued for patients and all this information is
  logged in hospital servers as per date.
  
  When a button which displays the patient visits against the type of day is 
  pressed

  Then a pie chart is displayed with the required content in it.

Scenario: Compute parking slots to reserve for visiting specialists

  Given we have two parking lots, one for staff & specialists and other for 
  visitors and patients
  
  When there is a specialist visiting the hospital
  
  Then the parking capacity is computed based on the staff present and a 
  slot is booked for the specialist
   