# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given the hospital has entry-card issuer
  When the visitor enters the hospital
  Then report visitor trends

Scenario: Alert when seating capacity is full

  Given the Hospital has seating facility
  When the number of available seats is zero
  Then Alert the facility team
