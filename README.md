### Cascade Assessment Project

##### To Create Database,
      Use CreateDb.Sql file by modifying database file and log file location in the file script file

##### To Create Tables and stored procs,
      Use Setup.Sql to create the tables and stored proedures

##### To insert test data,
      Use Insert_TestData.Sql

##### Source Code Details
      Visual Studio 2019 Solution 'Cascade.Assessment.Api.sln' contains two projects 
      Cascade.Assessment.Api.csproj and Cascade.Assessment.Db.sqlproj
      
      Cascade.Assessment.Api.csproj is .Net Core 3.1 Api Project
      
      Cascade.Assessment.Db.sqlproj is a database project and that can be used to 
      publish the database, tables and stored procs. 
      
##### Deploying the Database
      
      Database, tables and stored procs can be deployed from visual studio by publishing
      Cascade.Assessment.Db.sqlproj database project.
      
      Database, tables and stored procs can be created manually using CreateDb.sql and Setup.Sql script files.
      When creating using the script files, specify the location data and log files.
      
##### Inserting test data
      
      Insert_TestData.sql file has scripts to insert test data to the necessary tables
      
##### Testing the Api
      
      When you debug from Visual Studio, Swagger page opens up to be able to test the Api calls
      
![image](https://user-images.githubusercontent.com/76564982/160248823-12a058a7-f777-4e62-8c72-fe44776f62c5.png)

##### Large List of Books to saved to database in One call
      
      POST call with array of Books object will save the books in the database in one call
      
      Schema
      
      [
      {
        "publisher": "string",
        "title": "string",
        "subTitle": "string",
        "authorLastName": "string",
        "authorFirstName": "string",
        "price": 0,
        "minimumPages": 0,
        "maximumPages": 0,
        "publishedDate": "2022-03-26T16:38:59.806Z",
        "publishedLocation": "string",
        "bookEdition": "string"
      }
      ]
      
      
