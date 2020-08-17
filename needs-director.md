# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given we have unique cards issued for patients and hospital servers
  log this information per day.

  When the director presses the show button

  Then we will show a pie chart with the required content in it.

Scenario: Compute parking slots to reserve for visiting specialists

  Given we have two parking lots, one for staff & specialists and other for
  visitors and patients

  When there is a specialist visiting the hospital

  Then we compute the parking capacity based on the staff present and book
  a slot for the specialist
