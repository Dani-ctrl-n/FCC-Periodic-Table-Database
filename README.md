# Periodic Table Database

This project provides a PostgreSQL database dump named "periodic_table," capturing information about chemical elements and their properties.

## Database Structure

### 1. Elements Table

- `atomic_number` (Primary Key)
- `symbol`
- `name`

### 2. Properties Table

- `atomic_number` (Foreign Key referencing elements)
- `atomic_mass`
- `melting_point_celsius`
- `boiling_point_celsius`
- `type_id` (Foreign Key referencing types)

### 3. Types Table

- `type_id` (Primary Key)
- `type`

## Usage

1. **Install PostgreSQL:**
   - Ensure you have PostgreSQL installed on your system.

2. **Create Database:**
   - Create a database named "periodic_table" using the following command:

     ```sql
     CREATE DATABASE periodic_table;
     ```

3. **Connect to Database:**
   - Connect to the "periodic_table" database:

     ```sql
     \c periodic_table;
     ```

4. **Run SQL Script:**
   - Execute the provided SQL script to create tables and insert sample data:

     ```sql
     -- Replace with the actual path to your SQL script
     \i path/to/your/script.sql;
     ```

Feel free to explore the fascinating world of chemistry with this database!

## Notes

- This dump includes sample data for chemical elements and their properties.
- Ensure proper configuration and permissions are set according to your PostgreSQL setup.
- For any inquiries or issues, please contact the repository owner.
