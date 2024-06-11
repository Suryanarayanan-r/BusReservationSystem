# BusReservationSystem

This is a Java-based bus reservation system that allows users to book seats on a bus and check for availability based on the bus capacity at the booking office.


## Features
- Add bookings
- Check seat availability
- Display bus information

## Technologies Used
- Java
- MySQL
- JDBC



### Prerequisites
- Java Development Kit (JDK)
- MySQL Server
- An IDE (e.g., IntelliJ IDEA, Eclipse)

### Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Suryanarayanan-r/BusReservationSystem.git
   cd BusReservationSystem

### MySql
Open your MySQL client and run the following SQL commands to set up the database and tables:
CREATE DATABASE busresv;
```
USE busresv;

CREATE TABLE bus (
  id INT PRIMARY KEY,
  ac BOOLEAN,
  capacity INT
);

INSERT INTO bus VALUES (1, 1, 2), (2, 1, 48), (3, 0, 52);

CREATE TABLE booking (
  passenger_name VARCHAR(50),
  bus_no INT,
  travel_date DATE
);
```
### Changes
Open DbConnection.java and update the url, userName, and passWord fields with your MySQL database credentials:
```
private static final String url = "jdbc:mysql://localhost:3306/busresv";
private static final String userName = "yourUsername";
private static final String passWord = "yourPassword";
```
### How to run
Run the main class BusDemo to start the application and follow the prompts to book a bus ticket.

