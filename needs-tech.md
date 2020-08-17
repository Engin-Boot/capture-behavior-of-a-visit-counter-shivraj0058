# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given foot-fall sensor at the door
  When the server restarts
  Then Countinue with the previous counter
  
Scenario: Reconcile counts if the sensor is offline for a while

  Given foot-fall sensor at the door
  When the server is online
  Then Continue with the previous count
