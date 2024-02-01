Name - ABHINAV EMPATY
ID - 0848728

LAB 1

Date - 2024-01-17
Time - 1300

Step 1:

Create a web app using ASP.NET Core MVC and Visual Studio

Problem: 

The creating the account and setting up was bit hard at first and then I was able to follow the document.

Solution:

The document was the big bonus for us again, every micro details was important, so small small codes or data are important and after following that i was able to create it successfully.

Step 2:

Add a controller to an ASP.NET Core MVC application.

Problems:
How to name the controller class and the methods inside it?
How to use the scaffolding feature to generate a controller template?
How to specify the routing logic that maps the URL to the controller action?

Solution**:
The controller class should be named with the suffix "Controller", such as "HelloWorldController". The methods inside the controller class are called action methods, and they should have descriptive names that indicate their functionality, such as "Index" or "Welcome".
To use the scaffolding feature, right-click the Controllers folder in the Solution Explorer and select Add > New Scaffolded Item. Then, select MVC Controller - Empty and click Add. Enter the name of the controller class and click Add again. This will create a controller file with the basic code structure and a corresponding view folder.
To specify the routing logic, use the [Route] attribute on the controller class or the action methods. The [Route] attribute takes a parameter that defines the URL pattern that matches the controller or the action. For example, [Route("HelloWorld")] on the controller class means that any URL that starts with "HelloWorld" will be handled by this controller. [Route("Welcome")] on the action method means that the URL "HelloWorld/Welcome" will invoke this action.

Step 3:

Create a view for the Index action method of the HelloWorldController class that displays a welcome message and the current date and time.

Problems:
How to create a view file and associate it with a controller action method?
How to use Razor syntax to write dynamic HTML code in the view file?
How to pass data from the controller to the view?

Solutions:

1. In the Solution Explorer, right-click on the Views folder and select Add > New Folder. Name the folder HelloWorld.
2. Right-click on the HelloWorld folder and select Add > New Item.
3. In the Add New Item dialog, select Show All Templates.
4. In the search box in the upper-right corner, enter view.
5. Select Razor View - Empty and keep the default name Index.cshtml.
6. Replace the contents of the Views/HelloWorld/Index.cshtml 

***********************************************************************************

LAB 2

Date - 2024-01-25
Time - 1030

Step 4:

Add a model to an ASP.NET Core MVC app

Challenges:

In this tutorial, classes are added for managing movies in a database. These classes are the "Model" part of the MVC app.
These model classes are used with Entity Framework Core (EF Core) to work with a database. EF Core is an object-relational mapping (ORM) framework that simplifies the data access code that you have to write.
The model classes created are known as POCO classes, from Plain Old CLR Objects. POCO classes don't have any dependency on EF Core. They only define the properties of the data to be stored in the database.
In this tutorial, model classes are created first, and EF Core creates the database.

Solution:

The Builder file was running few erros, but i removed all data and again typed all from 
doc so that it runs properlly.

Step 5:

Work with a database in an ASP.NET Core MVC app

Challenges:

As I Delete all the records in the database. 
You can do this with the delete links in the browser or from SSOX.
Test the app. Force the app to initialize, calling the code in the Program.cs file,
so the seed method runs. To force initialization, close the command prompt window that 
Visual Studio opened, and restart by pressing Ctrl+F5.

Solution:

The program.cs file had the minor changes so I went to doc and read every line, and managed
to rewrite the code and all.

Finally Hurray it worked.

Step 6:

Challenges:

The edit and details and delete was new task to get the urls on the bottom left.
We were able to bring them. also the data in not in correct spacing format.

Solution:

The proper codes like:

using System;
using System.ComponentModel.DataAnnotations;
using System.ComponentModel.DataAnnotations.Schema;

Have slight changes and made them work at the end.

Eveything is linked to the program.cs file so again made the changes there and got the
correct output.

Migrations:

20240125052346_InitialCreate.cs

*******************************************************************************************

LAB 3

Date - 2024-02-01
Time - 0930

Step 7:

CHALLENGES:

i was able to work on search command but initially i was not able to run it.

Solution:

I was doing the task by imagine that you want to bookmark a particular search or you want to send
a link to friends that they can click in order to see the same filtered list of movies. Notice that 
the URL for the HTTP POST request is the same as the URL for the GET request (localhost:{PORT}/Movies/Index) 
-- there's no search information in the URL. 

Step 8:

challenges:

creating a new field R was coming errors.

solution:


Navigated to the relevant model class within the project. 
Added a new property to the class with the appropriate data type:
Added a new property in the model class, specifying the appropriate data type for the desired field.
Opened the data context class to add a new DbSet for the new property:
Accessed the data context class that is associated with the model and incorporated a new DbSet for the newly
added property.Actually i did not build the commands, but again i started from staring 8 step, so i got rating field in it.

Step 9:
Executed the migration to update the database with the new field.
Executed a migration to apply the changes to the database, ensuring synchronization with the updated model.
Updated the views and controllers to handle the new field.Modified the views and controllers that involve the model
to accommodate the new field, ensuring proper handling and integration into the application's user interface and
functionality.
Was able to run create page.
But cloning to git was having few errors.