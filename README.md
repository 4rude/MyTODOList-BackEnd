# MyTODOList - Back End
This is the backend portion of the MyTODOList application that I helped write with an Agile team. The application is a to-do list/event planner, created to help users plan out their day better. 

**I did not create the event class, however it is closely related to the SQLiteDBConnection class and SQLiteUtility class (which I was responsible for creating) so I decided to add that to the backend portion of this applicaiton.**

In the SQLiteDBConnection class there is one function named connectDB. This function is in charge of connecting the controller (MVC) to the model. It also houses the connection string for the SQLite database. The SQLiteDBConnection class is found under the model folder.

Within the SQLiteUtility class there are five core functions. These are:

1. retrieveEventFromDatabase
2. retrieveEventsFromDatabase
3. writeEventToDatabase
4. updateEventInDatabase
5. deleteEventFromDatabase

The functions are all written to allow for easy I/O to and from the database. The functions use the PreparedStatement java object to send data from the View to the SQLite database. The reason for using the PreparedStatement objects is because they precompile the SQL statements before being ran, so the DBMS doesn't have to. 

The database (event.db) holds the event information for each event that was inputted by the user. The SQLite database is found under the resources folder.

The full MyTODOList project can be found here: https://github.com/manicmachine/MyTODOList/blob/master/src/edu/cvtc/MyTODOList/model/SQLiteUtility.java


