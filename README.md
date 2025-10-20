
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

---

## Database Design
**Entities:**  
- **User:** id, username, email, password  
- **Property:** id, title, price, owner_id  
- **Booking:** id, user_id, property_id, check_in, check_out  
- **Review:** id, user_id, property_id, rating, comment  
- **Payment:** id, booking_id, amount, status  

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


