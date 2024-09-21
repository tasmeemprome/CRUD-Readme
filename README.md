
# CRUD Application - C# with SQL Database

This project demonstrates a simple CRUD (Create, Read, Update, Delete) operation in a C# application using a SQL database. The data in the table represents a list of users with their first and last names, along with a unique ID.



## Prerequisites

Before running this application, ensure that you have the following installed:


- Visual Studio (any version with C# support)
- SQL Server or SQL Server Express
- .NET Framework (version 4.7.2 or later)
- SQL Server Management Studio (SSMS) (optional but useful for database management)

## Database Setup
Step 1 : Generate Database Script
1. Open SQL Server Management Studio (SSMS).
2. Navigate to the `Database` section.
3. Right-click on the desired database (e.g., `task`).
4. Select Tasks > Generate Scripts.
5. Follow the on-screen instructions to generate a script for the table schema and data.
6. Save the generated SQL script in the project directory (e.g., `database/script.sql`).

Step 2 : Backup the Database (Optional)
1. In SSMS, right-click on the database (`task`).
2. Choose Tasks > Back Up.
3. Specify the destination for the backup file.
4. Save the backup in the project directory (e.g., `database/task_backup.bak`).

## How to Run

1. Clone the repository to your local machine:

```bash
  git clone https://github.com/yourusername/repository.git

```
2. Open the solution (`.sln`) file in Visual Studio.

3. Set up the database:

- Restore the database backup (optional):
- Open SSMS.
- Right-click on the Databases folder and select Restore Database.
- Choose the `task_backup.bak` file.
- Alternatively, run the SQL script to create the table:
- Open SSMS, and connect to your server.
- Open the `script.sql` file and execute it to create the table.

4. Modify the connection string in the app.config or web.config file:
```bash
  <connectionStrings>
  <add name="DatabaseConnection" connectionString="Data Source=LAPTOP-L8JGFSH4;Initial Catalog=MTPEOJECT;Integrated Security=True;TrustServerCertificate=True;" providerName="System.Data.SqlClient"/>
</connectionStrings>

```
Replace `LAPTOP-L8JGFSH4` with your actual SQL server name.

5. Build the project by clicking Build > Build Solution.

6. Run the application in Visual Studio.

## CRUD Operations
The application allows you to perform the following actions:

- Create: Add a new record (user) to the database.
- Read: View existing records.
- Update: Modify the details of a user.
- Delete: Remove a user from the database.

## Example Data

The table below shows an example of the data structure used in the application:
![Screenshot 2024-09-21 121941](https://github.com/user-attachments/assets/16e9578f-0bd3-418e-9d2a-1b0f299a9294)

## Support

For support, email tasmeemjannatprome@gmail.com or video link- https://youtu.be/1CeGA8k1sn4?si=9BHFwIKxPjuBS64I.


## License

[MIT](https://choosealicense.com/licenses/mit/)

