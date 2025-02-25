# GaudiDB - A SQL-Based Relational Database

## Overview
GaudiDB is a modular SQL-based relational database designed for learning and experimentation with database internals. The project implements core database features such as SQL parsing, query execution, indexing, and transaction management.

## Features
- **SQL Query Processing**: Supports basic SQL commands (`SELECT`, `INSERT`, `UPDATE`, `DELETE`)
- **Storage Engine**: Implements file-based storage and indexing (B-Trees, Hash Indexes)
- **Transaction Management**: Supports ACID properties
- **Query Optimization**: Basic query planner and optimizer
- **Modular Architecture**: Easily extendable and scalable
- **Gradle-Based Build System**

## Folder Structure
```
mydatabase/
│── build.gradle              # Gradle build file
│── settings.gradle           # Gradle settings
│── README.md                 # Project documentation
│── docs/                     # Design documentation
│── src/
│   ├── main/java/com/mydb/
│   │   ├── queryprocessor/   # SQL Parsing & Execution
│   │   ├── storage/          # Data Storage & Indexing
│   │   ├── transaction/      # ACID Transactions
│   │   ├── optimizer/        # Query Optimization
│   │   ├── networking/       # (Optional) Client-Server Support
│   │   ├── logging/          # Logging & Monitoring
│   │   ├── utils/            # Common utilities
│   │   └── MyDatabase.java   # Main entry point
│   ├── test/                 # Unit & integration tests
│   ├── resources/            # Config files, SQL examples
```

## Setup & Installation
### Prerequisites
- Java 17 or higher
- Gradle 8+

### Clone the Repository
```sh
git clone https://github.com/your-repo/mydatabase.git
cd mydatabase
```

### Build the Project
```sh
gradle build
```

### Run the Application
```sh
gradle run
```

### Running Tests
```sh
gradle test
```

## Usage
- **Create a Table**:
  ```sql
  CREATE TABLE users (id INT PRIMARY KEY, name VARCHAR(50));
  ```
- **Insert Data**:
  ```sql
  INSERT INTO users (id, name) VALUES (1, 'Alice');
  ```
- **Query Data**:
  ```sql
  SELECT * FROM users;
  ```

## Roadmap
- [ ] Implement advanced query optimization
- [ ] Add support for foreign keys and constraints
- [ ] Improve indexing and query caching
- [ ] Implement full transaction support with MVCC

## Contributing
Contributions are welcome! Please submit a pull request with a clear description of changes.

## License
MIT License

## Contact
For questions or suggestions, reach out to [your.email@example.com]

