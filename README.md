
#  Airbnb Clone Project — StayBackend

## Overview
The Airbnb Clone Project is part of the ALX Backend Blueprint. It simulates the backend of a booking platform like Airbnb, focusing on backend design, database structure, API security, and CI/CD practices.

---

## Team Roles
- **Backend Developer:** Builds APIs and core logic using Django.  
- **Database Admin:** Designs and maintains the MySQL database.  
- **Frontend Developer:** Connects APIs with the user interface.  
- **DevOps Engineer:** Manages Docker and CI/CD pipelines.  
- **Project Manager:** Coordinates tasks and ensures deadlines are met.  

---

## Technology Stack
- **Django:** Backend framework for RESTful APIs.  
- **MySQL:** Database for storing structured data.  
- **GraphQL:** Enables efficient data querying.  
- **Docker:** For containerization.  
- **GitHub Actions:** For CI/CD automation.  


# Database Design

## Entities

### 1. User
- id (Primary Key)
- username
- email
- password
- date_joined

### 2. Property
- id (Primary Key)
- title
- description
- price_per_night
- location
- owner_id (Foreign Key → User)

### 3. Booking
- id (Primary Key)
- user_id (Foreign Key → User)
- property_id (Foreign Key → Property)
- check_in_date
- check_out_date
- total_price

### 4. Review
- id (Primary Key)
- user_id (Foreign Key → User)
- property_id (Foreign Key → Property)
- rating
- comment

### 5. Payment
- id (Primary Key)
- booking_id (Foreign Key → Booking)
- amount
- payment_status
- payment_date

## Relationships
- A **User** can have multiple **Properties**.  
- A **Booking** belongs to one **Property** and one **User**.  
- A **Property** can have multiple **Reviews**.  
- A **Booking** can have one **Payment**.




  ## Feature Breakdown
- **User Authentication** – Handles login, signup, and password reset.
- **Dashboard** – Displays user-specific information after login.
- **Notifications** – Alerts users about new updates or tasks.
- **Reporting Module** – Generates detailed user activity reports.
- **Admin Panel** – Enables admins to manage users and settings.  

**Relationships:**  
- A user owns many properties.  
- A booking belongs to one property and one user.  
- A property can have many reviews.  
- Each booking has one payment.  

---

## Feature Breakdown
- **User Management:** Register, login, profile.  
- **Property Management:** Add/edit property listings.  
- **Booking System:** Book and manage stays.  
- **Review System:** Leave property feedback.  
- **Payment Handling:** Secure transactions.  

---

## API Security
- **Authentication & Authorization:** Verify and control access.  
- **Rate Limiting:** Prevent abuse.  
- **Input Validation:** Block SQL injection/XSS.  
- **HTTPS Encryption:** Secure data exchange.  

---

## CI/CD Pipeline
- **CI/CD:** Automates testing and deployment.  
- **Tools:** GitHub Actions, Docker.  
- **Benefits:** Faster updates, fewer errors, consistent environments.  

---


