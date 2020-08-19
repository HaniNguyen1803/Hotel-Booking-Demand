# Project Summary 
Hotel Booking Demand is a classification problem to predict the price range of a phone given its attributes.

# Dataset
The dataset can be found in [Kaggle](https://www.kaggle.com/jessemostipak/hotel-booking-demand).

# Attributes
- Numerical:
  - 'lead_time': Number of days that elapsed between the entering date of the booking into the PMS and the arrival date
  - 'arrival_date_year': Year of arrival date
  - 'arrival_date_week_number': Week number of the arrival date
  - 'arrival_date_day_of_month': Day of the month of the arrival date
  - 'stays_in_weekend_nights': Number of weekend nights (Saturday or Sunday) the guest stayed or booked to stay at the hotel.
  - 'stays_in_week_nights': Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel.
  - 'adults': Number of adults
  - 'children': Number of children
  - 'babies': Number of babies
  - 'previous_cancellations': Number of previous bookings that were cancelled by the customer prior to the current booking.
  - 'previous_bookings_not_canceled': Number of previous bookings not cancelled by the customer prior to the current booking .
  - 'booking_changes': Number of changes/amendments made to the booking from the moment the booking was entered on the PMS until the moment of check-in or cancellation.
  - 'days_in_waiting_list': Number of days the booking was in the waiting list before it was confirmed to the customer.
  - 'adr': Average Daily Rate
  - 'required_car_parking_spaces': Number of car parking spaces required by the customer.
  - 'total_of_special_requests': Number of special requests made by the customer (e.g. twin bed or high floor).
- Categorical:
  - 'hotel': Resort or City Hotel
  - 'is_canceled': Value indicating if the booking was canceled (1) or not (0)
  - 'arrival_date_month': Month of arrival date with 12 categories: “January” to “December”.
  - 'meal': Type of meal booked. Categories are presented in standard hospitality meal packages:
    - Undefined/SC – no meal package;
    - BB – Bed & Breakfast;
    - HB – Half board (breakfast and one other meal – usually dinner);
    - FB – Full board (breakfast, lunch and dinner)
  - 'country': Country of origin. Categories are represented in the ISO 3155–3:2013 format.
  - 'market_segment': Market segment designation. In categories, the term “TA” means “Travel Agents” and “TO” means “Tour Operators”
  - 'distribution_channel': Booking distribution channel. The term “TA” means “Travel Agents” and “TO” means “Tour Operators”
  - 'is_repeated_guest': Value indicating if the booking name was from a repeated guest (1) or not (0)
  - 'reserved_room_type': Code of room type reserved. Code is presented instead of designation for anonymity reasons.
  - 'assigned_room_type': Code for the type of room assigned to the booking. Sometimes the assigned room type differs from the reserved room type due to hotel operation reasons (e.g. overbooking) or by customer request. Code is presented instead of designation for anonymity reasons.
  - 'deposit_type': Indication on if the customer made a deposit to guarantee the booking. This variable can assume three categories:
    - No Deposit
    - Non Refund – a deposit was made in the value of the total stay cost;
    - Refundable – a deposit was made with a value under the total cost of stay.
  - 'agent': ID of the travel agency that made the booking
  - 'company': ID of the company/entity that made the booking or responsible for paying the booking. ID is presented instead of designation for anonymity reasons.
  - 'customer_type': Type of booking, assuming one of four categories:
    - Contract - when the booking has an allotment or other type of contract associated to it;
    - Group – when the booking is associated to a group;
    - Transient – when the booking is not part of a group or contract, and is not associated to other transient booking;
    - Transient-party – when the booking is transient, but is associated to at least other transient booking
  - 'reservation_status': Reservation last status, assuming one of three categories:
    - Canceled – booking was canceled by the customer;
    - Check-Out – customer has checked in but already departed;
    - No-Show – customer did not check-in and did inform the hotel of the reason why
  - Date: 'reservation_status_date': Date at which the last status was set. This variable can be used in conjunction with the ReservationStatus to understand when was the booking canceled or when did the customer checked-out of the hotel

# Process
1. Data Preprocessing
- Convert NULL/ Undefined values
- Handle missing data
- Delete wrong values
- Handle Date
2. Data Exploration
- General view of hotel booking demand
  - Monthly and yearly booking
  - General Lead Time
  - Average stay time
  - Country of bookings
  - What attributes affect cancellations?
- Compare Resort Hotel with City Hotel
