# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given the hospital has entry-card issuer
  When patient visits the hospital
  Then show patient visits

Scenario: Compute parking slots to reserve for visiting specialists

  Given the Hospital has Staff attendance system
  When the specialist is going to visit
  Then find the parking slots available
