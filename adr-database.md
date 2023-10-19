# Architecture Decision Record for Study Planner App
**Decision Title:** Selection of Database

**Date:** Oct 18, 2023

**Team members:** Matthew Yackel, Sergei Mochalov, Steph Martyna, Martin Contreras

## Background
The storage system of the app will define where the data will be processed, where the data will be stored, and how the data will be stored. The team must consider wether the data will be stored locally or remotely and if the data needs encryption.

## Decision
The team has decided on the solution of the SQLite database.

## Reasoning 
**React Native compatibility**
   - 

**Structured data**
   - 

**performance**
   - 

**lightweight**
   - 

**FOSS**
   - 

## Consequences
   - No sync
   - collaboration development complexity

## Conclusion
<!-- NOT FINAL, NEEDS REVISION -->
Selecting SQLite as our local database for the Study Planneer app is a robust choice that aligns well with our requirements. While it may introduce some complexity, the benefits of performance, compatibility, and widespread adoption outweigh the challenges. We will provide necessary training and documentation to ensure the team is equipped to work with SQLite effectively. Proper maintenance procedures will be implemented to ensure data integrity and longevity.