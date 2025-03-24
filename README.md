# Hotel Management System

## Overview
The Hotel Management System is a Java-based application that simplifies and automates the management of hotel services such as room booking, food service, and guest management. This system can be used by hotel staff to efficiently manage room availability, food orders, and customer information.

## Features
- **Room Management**: Includes functionalities for both single and double rooms. It allows users to book, check availability, and manage rooms.
- **Food Management**: Manages food services provided by the hotel.
- **Customer Management**: Handles guest information such as personal details, room assignments, and billing.
- **Availability Check**: Ensures that rooms are available or not before proceeding with booking.

## Project Structure

Here's a breakdown of the project structure:

```
HotelManagementSystem/
├── src/main/java/
│   ├── DoubleRoom.java        # Class to manage double rooms
│   ├── Food.java              # Class to handle food services
│   ├── Holder.java            # Represents a guest or holder in the system
│   ├── Hotel.java             # Core hotel management functionalities
│   ├── Main.java              # Main entry point of the system
│   ├── NotAvailable.java      # Handles room unavailability situations
│   ├── Service.java           # Service functionality related to hotel services
│   ├── SingleRoom.java        # Class to manage single rooms
│   └── Write.java             # Class to handle file writing (data persistence)
├── target/classes/           # Compiled classes after building the project
├── backup/                   # Backup of previous versions or data
├── pom.xml                   # Maven configuration file
├── Hotel Management System SDS.docx # Software Design Specification
├── Hotel Management System SRS.docx # Software Requirement Specification
└── README.md                 # Project documentation (this file)
```

## Installation

To run the Hotel Management System locally, follow these steps:

### Prerequisites
- **Java 8 or higher**
- **Maven** (for dependency management and building the project)

### Steps to Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/HotelManagementSystem.git
   ```

2. Navigate into the project directory:
   ```bash
   cd HotelManagementSystem
   ```

3. Install dependencies using Maven:
   ```bash
   mvn install
   ```

4. Build the project:
   ```bash
   mvn clean package
   ```

5. Run the application:
   ```bash
   java -cp target/classes Main
   ```

## Classes and Functionalities

### `Main.java`
- The entry point of the application that runs the system and manages user interactions.

### `Hotel.java`
- This class encapsulates the core functionalities for managing the hotel, such as adding/removing rooms, checking room availability, etc.

### `DoubleRoom.java` and `SingleRoom.java`
- These classes represent the room types in the hotel. They allow functionalities such as booking, availability checking, and pricing.

### `Food.java`
- Handles food-related services and operations such as menu management and food orders.

### `Service.java`
- Manages hotel services like room cleaning, maintenance, etc.

### `Holder.java`
- Represents a guest or user who can book rooms and order services.

### `NotAvailable.java`
- This class is used when rooms are unavailable. It helps in handling exceptions related to room booking.

### `Write.java`
- A utility class that handles file writing, likely used for saving guest data or room availability to disk.

## Documentation

- **Hotel Management System SDS**: Contains the software design specifications and outlines the system architecture and implementation details.  
- **Hotel Management System SRS**: Contains the software requirement specifications and outlines the system's functional and non-functional requirements.

## Usage

Once the application is up and running, you can interact with it through a command-line interface (CLI). The system allows you to:
1. View room availability.
2. Book rooms (single or double).
3. Order food services.
4. Manage customer information and hotel services.

### Example:

1. **Booking a Single Room**:
   - User enters the desired check-in and check-out dates.
   - The system checks availability and processes the booking.

2. **Food Ordering**:
   - User can order food from the menu, and the system calculates the total cost.

3. **Service Request**:
   - The user can request services such as cleaning or room service.

## Contributing

If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

## License

This project is open-source and available under the [MIT License](LICENSE).
