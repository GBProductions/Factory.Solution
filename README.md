# _Dr. Sillystringz's Factory_

 * _A program to allow Dr. Sillystringz's Factory to keep track of Engineers and Machines._
 * _Date Created: June 4th 2021_
 * _Date Updated: June 10th 2021_

#### By _**Garrett Brown**_

## Description
_A program that allows Dr. Sillystringz's Factory to keep track of Engineers and Machines. Users can create Engineers, Machines, and assorted details. Users can also keep track of which Machines are assigned to which Engineers, and vice versa. Users can also edit or delete details for Engineers, or Machines._

### User Stories

<details>
    <summary>Expand</summary>

#### User Stories
As the factory manager, I need to be able to see a list of all engineers, and I need to be able to see a list of all machines.
As the factory manager, I need to be able to select a engineer, see their details, and see a list of all machines that engineer is licensed to repair. I also need to be able to select a machine, see its details, and see a list of all engineers licensed to repair it.
As the factory manager, I need to add new engineers to our system when they are hired. I also need to add new machines to our system when they are installed.
As the factory manager, I should be able to add new machines even if no engineers are employed. I should also be able to add new engineers even if no machines are installed
As the factory manager, I need to be able to add or remove machines that a specific engineer is licensed to repair. I also need to be able to modify this relationship from the other side, and add or remove engineers from a specific machine.

</details>

## Setup/Installation Requirements
Table of Contents
* Required Programs
* Installation of Program
* Recreate Database
* Startup

<details>
    <summary>Expand for Instructions</summary>

### Required Programs
1. An internet browser.
2. Visual Code Studio (or another code editor).
3. .NET
4. MySQL
5. MySQLWorkbench


### Installation of Program
* _Open the terminal on your local machine and navigate to "Desktop."_
* _Clone "Factory.Solution"" with the following git command `git clone https://github.com/GBProductions/Factory.Solution.git_`
* _Navigate to the top level of the repository with the command `cd Factory.Solution`_
* _Navigate into "Factory" with git command `cd Factory`_


### Recreate Database

#### Instructions: `appsettings.json` Creation

1. Create a file in the root directory called `appsettings.json`. 
2. Add `appsettings.json` to `.gitignore`.
3. Insert the following code into `appsettings.json`:
    
``` 
{
    "ConnectionStrings": {
        "DefaultConnection": "Server=localhost;Port=3306;database=YOUR-DATABASE;uid=root;pwd=YOUR-PASSWORD;"
    }
}
```

4. Replace `YOUR-PASSWORD` with password you selected when installing MySQLWorkbench.
5. Replace `YOUR-DATABASE` with the name of your database.
6. In the root directory, run `dotnet ef databse update` 
7. In the root directory, run `dotnet ef databse restore`

This will recreate the database on your computer, using MySQLWorkbench. You can proceed to Startup.



### Startup
* Navigate to root directory in project.
* Restore project with git command `dotnet restore`
* Build project with git command `dotnet build`
* To run program, run git command `dotnet run`
* In browser, navigate to http://localhost:5000 

</details>

## Known Bugs

_There are currently no known bugs._

## Support and contact details

_For assistance, please contact Garrett Brown <garrettpaulbrown@gmail.com>_

## Technologies Used

* _Github, VS Code_
* _Bootstrap, MarkDown_
* _Entity Framework_
* _C#_
* _.NET Core 5.0.1_
* _ASP.NET Core MVC_
* _ASP.NET Core Razor Pages_
* _HTML, CSS_
* _MySQL_
* _MySQLWorkbench_


### License

*Available under MIT Licensing*

Copyright (c) 2021 **_Garrett Brown_**

