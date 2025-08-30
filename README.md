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
