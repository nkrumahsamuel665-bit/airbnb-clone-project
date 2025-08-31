# airbnb-clone-project
A  simplified AirBnB clone built to practice full-stuck web development.
## Overview
This project is a simplified clone of the AirBnB platform.  
It is built to help understand the fundamentals of *full-stack web development*,  
covering backend, database management and deployment.

## Project Goals
- Build a command-line interpreter for managing AirBnB objects.  
- Implement storage engines (JSON file and MySQL database).  
- Develop a dynamic web framework using Flask.  
- Create RESTful APIs for communication.  
- Deploy the project for production use.

## Tech Stack
 *Python* – Backend logic  
 *Flask* – Web framework  
 *MySQL* – Database   
 *Git/GitHub* – Version control  
*Docker* (optional) – Deployment

## Author
- Samuel Nkrumah (nkrumahsamuel665-bit)

## Team roles
- **Project manager** -The project manager oversees the entire project.
- **Backend developer** -The back-end developer is responsible for building and managing the server-side of the AirBnB Clone.
- **Database administrator** -They ensure that the data backbone of the AirBnB Clone is reliable, secure, and efficient.
- **UI/UX Designer** -They create mockups and wireframes for a user-friendly experience
- **DevOps Engineer** -They handle deployment(docker) -They ensure scalability ,monitoring and system reliability.

## Database Design  
### Key Entities and Fields  

1. *Users*  
   - id 
   - name  
   - email  
   - password  
   - date_joined  

2. *Properties*  
   - id   
   - title  
   - description  
   - location  
   - price_per_night  

3. *Bookings*  
   - id   
   - start_date  
   - end_date  
   - status (e.g., confirmed, pending, canceled)  

4. *Reviews*  
   - id  
   - rating  
   - comment  
   - date_posted  

5. *Payments*  
   - id   
   - amount  
   - payment_method  
   - payment_status  
   - date_paid  


### Entity Relationships  

- A *User* can own multiple *Properties*.  
- A *Property* can have multiple *Bookings*.  
- A *Booking* belongs to one *User* and one *Property*.  
- A *Review* is written by a *User* for a specific *Property*.  
- A *Payment* is tied to one *Booking*.

  ## Technology Stack  

- *Django* – Backend framework for building the application logic and APIs.  
- *PostgreSQL* – Relational database to store users, properties, bookings, and payments.  
- *GraphQL* – Enables flexible and efficient data queries between frontend and backend.  
- *React* – Frontend library for building a user-friendly and interactive interface.  
- *Docker* – Used for containerization and easy deployment.  
- *Git & GitHub* – For version control and collaboration.

  ## Feature Breakdown  

### 1. User Management  
Handles user registration, login, and profile management. This feature ensures secure authentication and allows users to manage their personal information.  

### 2. Booking System  
Allow guests to search for properties, check availability, and make reservations. It connects users with hosts and manages booking confirmations.  

### 3. Property Management  
Enable hosts to list, update, and manage their properties. This feature ensures accurate property details, pricing, and availability for guests.  

### 4. Reviews & Ratings  
Allow guests leave reviews and ratings for properties they have booked. This feature builds trust and helps future guests make informed choices.  

### 5. Payment Integration  
Supports secure processing of payments between guests and hosts. It ensures smooth financial transactions and booking confirmations.

## API Security  
To ensure the safety of users and the integrity of the platform, the backend APIs will implement the following security measures:  

### 1. Authentication  
Only registered users can access protected endpoints using secure login credentials or tokens.  
➡ This protects user accounts and ensures only verified users interact with the system.  

### 2. Authorization  
Different roles (e.g., host, guest, admin) will have specific permissions.  
➡ This prevents unauthorized access, such as a guest trying to manage properties they do not own.  

### 3. Rate Limiting  
Limits the number of requests a user or client can make within a set time.  
➡ This protects the system against abuse and denial-of-service (DoS) attacks.  

### 4. Data Encryption  
Sensitive data, like passwords and payment details, will be encrypted in storage and during transfer.  
➡ This ensures privacy and protects financial transactions.  

### 5. Input Validation & Sanitization  
All inputs will be validated to prevent injection attacks (e.g., SQL injection, XSS).  
➡ This ensures the database and system remain secure.

## CI/CD Pipeline  
CI/CD pipeline is the continuous Integration and Continuous Deployment (CI/CD) pipelines which automate the process of testing, building, and deploying the application. They help ensure that new changes are integrated smoothly, tested automatically, and deployed with minimal errors.  

### Why CI/CD is Important  
- *Reliability:* Ensures code changes are tested before reaching production.  
- *Speed:* Automates repetitive tasks, reducing deployment time.  
- *Collaboration:* Helps multiple developers work on the project without conflicts.  
- *Consistency:* Ensures each deployment follows the same process, reducing human error.  

### Tools We Can Use  
- *GitHub Actions:* Automates testing and deployment directly from GitHub.  
- *Docker:* Ensures consistent environments across development and production.  
- *Heroku/AWS:* Can be used as hosting platforms for deploying the application.
