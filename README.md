# Hospital Bed Availability System

## 1. Project Overview
The Hospital Bed Availability System is a web-based platform designed to provide real-time information on bed availability across hospitals. It enables patients to check and book beds online, reducing delays and confusion during emergencies.

## 2. Problem Statement
During peak times and health crises, patients struggle to find available hospital beds. There is no centralized system to check bed status before visiting a hospital.  
This project aims to solve that by providing a transparent system where hospitals can update bed counts and patients can book beds in advance.

## 3. Tech Stack
- **Frontend**: HTML5, CSS3
- **Backend**: Python, Flask Framework
- **Database**: SQLite
- **Version Control**: Git, GitHub
- **Diagramming**: Mermaid.js

## 4. Key Features - MVP
1.  **User Authentication**: Separate login for Patients and Hospital Admins
2.  **Patient Module**: View available beds and book a bed in a hospital
3.  **Admin Module**: Hospital admins can update total and available bed counts
4.  **Booking Management**: Track all patient bookings in the database

## 5. Database Design
The system uses 3 main entities: `Users`, `Hospitals`, and `Bookings`.  
ER Diagram and Class Diagram are available in the `/docs` folder.

## 6. How to Run the Project
```bash
# 1. Clone the repository
git clone https://github.com/asubha227-ux/hospital-bed-availability-system.git

# 2. Install dependencies
pip install flask

# 3. Run the application
python app.py

# 4. Open in browser
http://127.0.0.1:5000
