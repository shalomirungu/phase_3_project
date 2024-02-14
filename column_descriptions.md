Churn: Indicates if the customer has stopped doing business with SyriaTel. (False = No churn, True = Churned)

State: The U.S. State of the customer. (Requires one-hot encoding; not ordinal)

Account Length: A smaller number signifies an older account. (Indicative of Customer Lifetime Value)

Area Code: The area code of the customer's phone number.

Phone Number: The customer's phone number.

International Plan: Whether the customer has an international plan. ('yes' or 'no'; binary and thus effectively one-hot encoded)

Voice Mail Plan: Whether the customer subscribes to a voice mail plan. ('yes' or 'no'; as above)

Number of Voice Mail Messages: Total number of voice mail messages left by the customer.

Total Day Minutes: Aggregate of daytime minutes used.

Total Day Calls: Total number of calls made during the day.

Total Day Charge: Total charges incurred for daytime calls.

Total Eve Minutes: Total minutes spent on calls in the evening.

Total Eve Calls: Number of calls made during the evening.

Total Eve Charge: Charges for evening calls.

Total Night Minutes: Total minutes for nighttime calls.

Total Night Calls: Number of calls made at night.

Total Night Charge: Nighttime call charges.

Total Intl Minutes: Cumulative international minutes (covering day, evening, and night).

Total Intl Calls: Total number of international calls (across all periods).

Total Intl Charge: Total charges for international calls.

Customer Service Calls: Number of calls made to customer service by the customer.

Target Variable Description:
Churn: if the customer has churned (true or false)
