In this assignment we are going to built Bookstore app.
We are doing Part 1
Doing in ASP.NEt Core Web Application
After chnaging the authentication type we are about to create the project now.
After creating the base of project we can clearly see Models, Views folders with HomeController.cs and some cs.html files.
5:40

In startup.cs file changing some 
In HomeController.cs file changing some elements of IActionresult
adding javascript file in layout.cshtml file which was given
After completing debugging 
we can see the welcome page with Home and Privacy
Now we will add some layouts and change some designs.
on the site of Bootswatch.com I selected a theme called Darkly and copied the bootstrap.css file and applied to my project.
By replacing the existing file of bootstrap to the new one which can be found under lib 
Changed Nav bar
run the project 
In a _layout.cshtml under views we added dropdown to NavBar
saved.
2022-11-04

after getting marks of part 1 i started working on my remaining part of part 1 which was not completetd.
added new three projects and named them virajbooks.Models, virajbooks.DataAccess and virajbooks.Utility.
deleted Data folder from Utility and copied it to DataAccess file.
Renamed the folder under virajbooks.Models to ViewModels.
deleted migration folder
but having errors in HomeController.cs on line 34 about namespace.
errors in Error.cshtml for the using statements
2022-11-10

We built the application and confirmed that there were no errors.
Reviewed the appsetting.json file
Migration added after getting error message from the package manager console that the target project doesn't match.
changed the default project.
New Migration Added.
2022-11-12 
9:58

Added new table to the DB by creating a Category model and pushed to the DB.
Added Migration - 20221113025410_AddDefaultIdentityMigration
Added using statement in ApplicationDbcontext.cs
Re-run the add-migration and got error that says"AddCategoryToDb" is used by an existing migration.
Removed the migration by using command inconsole.
then Updated the database.
build started...
build succeeded.
2022-11-12

started part2.2
clean and build the application
no errors found
created the category.cs file and added to the ApplicationDbContext.
added a folder called Repository and created another folder in it as Irepository
added type interface and named it Irepository.cs
modified files as per the tutorial
included using statement and implemented interfaces
Modified code to set contructors 
Now, its time to create individual repos Category.cs and ICategory.csModified ICategoryRepository.
Completed remaining modifications
having errors in Icategory as it shows formal parameter 'db' in file CategoryRepository.cs
Build the application and commited to GitHub.
Now we are going to implement the store procedure repository in Unit of work
Added a new interface in IRepository
and named it as ISP_Call.cs
having error in ISP_Call.cs then solved by installing  NuGet package
when having issue with Dynamic parameters then add nuget package Dapper with using statement
Implemented new class in the repository
Added new class in Repositroy, named it as SP_Call.cs
Using appropriate statements we implemented ISP_Call interface.
Added Connection.
Adding new interface called IUnitOfWork to IRepository folder.
updated the code with modifications.
Now intertesting part comes..... we are adding class in Repository folder as UnitOfWork 
Modified the code by adding ConfigureService method to be registered in Startup.cs

facing errors in sratup.cs as it says IUnitOfWork and UnitOfWork namespace could not be found
2022-11-13



