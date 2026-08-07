# Problem Statement

## 1. Title
Hospital Bed Availability and Booking System Across Multiple Hospitals

## 2. Domain
Healthcare / Hospital Management

## 3. Who is the user? (2-3 user types)
1. **Patient/Attender**: Can search for available beds by type and location, and book a bed.
2. **Hospital Admin**: Can update bed availability, add new beds, and manage bookings.
3. **Guest User**: Can only search and view bed availability.

## 4. What problem are we solving?
During emergencies, people waste critical time calling multiple hospitals to check for ICU, General, or Oxygen bed availability. There is no centralized platform to see real-time bed status. For example, a patient needing an ICU bed in Coimbatore doesn't know which hospital has vacancy. This delay can be life-threatening. Our system provides a single platform to check live bed status and book instantly.

## 5. Proposed Solution
The application will allow users to:
1.  Search hospitals by city and bed type: ICU, General, Oxygen, Ventilator.
2.  View real-time available bed count for each hospital.
3.  Book a bed for a patient with basic details.
4.  Hospital Admin can login and update bed count every few hours.
5.  Show contact number and address of hospital.

## 6. Core Entities / Database Tables
1.  **Patient**: patient_id, name, age, contact, address
2.  **Hospital**: hospital_id, name, address, city, contact
3.  **Bed**: bed_id, hospital_id, bed_type, total_count, available_count
4.  **Booking**: booking_id, patient_id, hospital_id, bed_id, booking_date, status
5.  **User**: user_id, email, password, role

## 7. User Roles & Permissions
1.  **Admin/Hospital**: Can update bed count, view all bookings for their hospital.
2.  **Patient**: Can search, book beds, and view own booking history.
3.  **Guest**: Can only search bed availability.

## 8. Success Criteria
1.  User should see bed availability of all hospitals in a city within 3 seconds.
2.  Booking a bed should reduce the available_count immediately.
3.  Admin should be able to update bed count and it reflects instantly.

## 9. Out of Scope
1.  Online payment for booking.
2.  Ambulance booking feature.
3.  Mobile app - Web application only for Phase 1.
