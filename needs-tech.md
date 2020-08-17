# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given there is a mechanism to auto-backup visit-counter for every update.

  When there is server a restart due to technical issue

  Then we recover the latest visit-counter from the auto-backup

Scenario: Reconcile counts if the sensor is offline for a while

  Given there is a mechanism to store visit-counter in the cloud

  When the sensor is online again

  Then we update the cloud value automatically with the latest count.
