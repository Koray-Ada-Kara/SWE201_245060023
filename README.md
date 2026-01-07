# Vehicle Rental Application (Toy Project)

This project is a sample console-based Python application that imitates
the operations of a vehicle rental company.

Its main goal is to demonstrate object-oriented design principles,
not to model a full real-world rental system.

## Design Principles

- Each class represents a real-life entity
- Classes store only the minimum required information
- Identifying data and operational state are clearly separated
- Business logic is handled by a manager class
- Model classes do not depend on user interface logic

## Classes

### RentalVehicle
Represents a vehicle owned by the company.
Stores identifying information (plate number, type) and operational state
(rental status and rates).

### RentalRequest
Represents a customer's request.
Contains only the requested vehicle type, request number, and request time.
It does not store vehicle information.

### RentalContract
Represents a temporary agreement between the customer and the company.
It links a request and a vehicle using identifiers rather than object references.

### RentalManager
Handles operations such as creating requests, assigning vehicles,
and managing contracts.

## Architecture

This project follows a simplified Model-based design.
In a real-world application, the same model classes could be reused in
desktop or mobile applications following the MVVM architecture.
