# Architecture Decision Record for Study Planner App
**Decision Title:** Selection of Database

**Date:** Oct 18, 2023

**Team members:** Matthew Yackel, Sergei Mochalov, Steph Martyna, Martin Contreras

## Background
The storage system of the app will define where the data will be processed, where the data will be stored, and how the data will be stored. The team must consider whether the data will be stored locally or remotely and if the data needs encryption.

## Decision
The team has decided on the SQLite database as the solution.

## Reasoning 
- **React Native compatibility**
SQLite is compatible with React Native by offering a JavaScript interface for React Native, which reduces project complexity and development time.

- **Structured Data**
<!-- COMPARE TO CouchDB -->
SQLite is a relational database, which allows the team to define tables and data structures to orginanize and manage data efficiently. 

- **Performance**
SQLite is considered to be a high-performance database. It offers fast data retrieval and manipulation. These aspects improve the user experience by quickly loading and storing data.

- **Lightweight**
SQLite is a lightweight and self-contained database system. It does not require a separate server or complex setup, which simplifies deployment and maintenance. 

- **FOSS**
SQLite is Free Open Source Software (FOSS). This ensures that the team can use SQLite without incurring licensing costs, and it provides the flexibility to customize and modify the database as needed.

## Consequences
- **collaboration development complexity**
Since SQLite is a local database, collaboration complexities may arise during development in terms of data syncronization. The team must adhere to proper version control and data migration strategies during the development process to ensure efficient collaborative development.

- **Backup and Recovery**
SQLite lacks backup and recovery features which are crusial for data integrity and data security. 

## Conclusion
<!-- INCLUDE COMPARISON TO CouchDB -->
By choosing SQLite as the storage solution for the app, the team has prioritized compatibility with React Native, structured data management, high performance, simplicity, lightweight deployment, and adherence to FOSS principles. While this decision offers numerous advantages, it also comes with the trade-offs of minimal data backup and recovery features and potential complexities in collaborative development. The team should carefully plan and address these consequences during the development process to ensure a successful and efficient app.