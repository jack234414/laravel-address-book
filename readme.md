# Laravel Assignment - Address Book Application (07/04/22)

## Requirements
Create a very basic address book application using Laravel. The application should <mark>show a listing of current address book entries (contacts), as well as having a way to edit existing contacts, create new contacts, and delete contacts.</mark> You should use a MySQL database (you will need to create the laravel migrations) and store the following data for a contact:
- Name
- Email
- Phone number
- Date of birth
- Physical address

You should create your own git repository for this project and commit your progress often as you work, to show your process. Please provide the URL to this repository when you are happy to share your progress.

**Optional ideas beyond the minimum requirements:**
- You could use a laravel starter kit (i.e. Laravel jetstream with VueJS - https://laravel.com/docs/9.x/starter-kits)
- <mark> You could implement an authentication flow to keep the application secure </mark> (tip: laravel jetstream and other starter kits come with this baked in)
- You could use laravel sail for an easier local development environment for PHP and MySQL
- You could utilise Tailwind CSS and TailwindUI for a better aesthetic


## Thoughts before starts

* CRUD function needed
* MySQL database
* UI wireframe
* Login page

## Current envir
* Laravel 
* php 8.0
* MySQL 8.0.15
* 

discussed a built web crwaler platform - Rstudio and its packages which uses to connect database. [R studio server](http://40.78.152.220:8787/)
usr: rstudio
pwd: rstudio

```php=8.0
# R
library(DBI)
library(RMySQL)

con <- dbConnect(RMySQL::MySQL(), 
    host = "ara-mysql.mysql.database.azure.com",
    user = "ara_user@ara-mysql", 
    password = "Test1234",
    dbname = "uml_resource"
)

dbListTables(con)
dbListFields(con, "webCrawler")
dbReadTable(con, "webCrawler")
```

**Done:**
* Can scrape a website and convert its content to an transferable format for database.
* Can create a table in MySQL by directly parsing the data in R studio.
* Run a prototype application by using Shiny package in R studio.

**Problem:**
* How to display/use data? 
* 1. Embed the Shiny application to React or .NET website.
* 2. Passing the stored data to website by 
* legltimate or not.


---
## Achievement and Issues
- [ ] Which method we use to collect data, collecting data through API or using web crawler?
- [ ] Where do we put the data, local MSSQL, Azure cloud-based SQL server or other tech.
- [ ]  A project design diagram/flow chart/mindmpa is considerably required. The following is an example.![](https://i.imgur.com/pYrmrev.png)

- [ ] A list of what tools or techniques we use, and what are they used for.


---
## A temporary List of Tools or Techniques
format: [Name, Simple description]

* [**Postman**, a platform for API development](https://www.postman.com/)
* **Front end language**: React or Vue
* **Backend language**: MS SQL, .NET Core
* **Web Crawler**: Python


---
# Resource
format: [Website, Title]
**Online Course**
1. [Lynda, Building React and ASP.NET MVC 5 Applications](https://www.lynda.com/ASP-NET-tutorials/Building-React-ASP-NET-MVC-5-Applications/751345-2.html)
2. [Microsoft, Virtual Training Days](https://www.microsoft.com/en-ca/sites/microsoft-training-days/azure.aspx)
3. [Python, Web Crawler Fundamental tutorial(Chinese)](https://drive.google.com/drive/folders/1Io8yX4F2p4TM4wdLD0O94EHefhcHawI3?usp=sharing)
4. [Coursera, Free cources for Uni. students](https://www.coursera.org/for-university-and-college-students?utm_source=link&utm_medium=share&utm_campaign=social_icons_freecourseraforstudents)

**Useful Reference**
1. [Microsoft, Tutorial: Create a web API with ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-3.1&tabs=visual-studio)
2. [Microsoft, Quickstart: Use .NET Core (C#) to query a database in Azure SQL Database or Azure SQL Managed Instance](https://docs.microsoft.com/en-us/azure/azure-sql/database/connect-query-dotnet-core)