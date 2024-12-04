# Airline Database Management System

A comprehensive SQL database system for managing airline operations, including flight scheduling, booking management, and passenger information.

## Features

- Airport and route management
- Aircraft fleet tracking
- Flight scheduling
- Passenger booking system
- Seat inventory management
- Fare class configuration

## Database Schema

The system includes these core tables:
- `airports`: Airport information and locations
- `aircraft`: Fleet management and capacity
- `flights`: Flight schedules and status
- `fare_classes`: Ticket classes and benefits
- `seats`: Aircraft seating configuration
- `passengers`: Customer data
- `bookings`: Reservation records

## Installation

1. Install PostgreSQL 12 or higher
2. Clone this repository
3. Run the schema creation script:
```bash
psql -U your_username -d your_database -f schema.sql
```

## Usage Examples

Query available flights:
```sql
SELECT * FROM flight_schedule 
WHERE departure_city = 'New York' 
AND arrival_city = 'London';
```

Check seat availability:
```sql
SELECT * FROM available_seats 
WHERE flight_id = 'FL123';
```

## Requirements

- PostgreSQL 12+
- 100MB minimum storage
- Basic SQL knowledge

## Contributing

1. Fork the repository
2. Create a feature branch
3. Submit a pull request

## License

Open source under MIT License

## Contact

For support or contributions, please open an issue in the repository.
