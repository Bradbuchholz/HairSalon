# Hair Salon
_By Brad Buchholz_
## Description

### _Eau Claire's Salon_
_You've been referred by Pierre to his friend Claire who is the owner of a hair salon called Eau Claire's Salon. She has contracted you out to create an MVC web application to help her manage her employees (stylists) and their clients. Claire should be able to add a list of stylists working at the salon, and for each stylist, add clients who see that stylist. The stylists have specific specialties, so each client can only see (belong to) a single stylist._

## Technologies Used 
* C#
* dotnet
* .Net 5.0
* HTML
* CSS
* MYSQL
* Markdown   

## Setup / Installation 

1. Download and install **`dotnet 5.0`** on your computer. 
2. Clone the GitHub [repository](https://github.com/Bradbuchholz/HairSalon.git) onto your computer.
3. Navigate to the directory via teriminal and use the command **`code .`** to open the program in your code editor.
4. Create an `appsettings.json` file in the `HairSalon/HairSalon/` directory and add the following code, replacing anything in `square brackets` with the information it represents specific to the project database: 
```
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database=[DATABASE-NAME-HERE];uid=[USER-ID-HERE];pwd=[YOUR-PASSWORD-HERE];"
  }
}

```
#### Example of complete appsettings.json
```
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database=hair_salon;uid=Myusername;pwd=MySuperStrongPassword;"
  }
}
```
5. Open MySql Workbench and login to your server. Click on the Administration tab in the Navigator on the left side of the screen. (this tab will likely be on the bottom of the window).
6. n the management section of this administration tab click on the button called **`Data Import/Export`**. Once the data import window opens click on **`Import from Self-Contained file`**, navigate into the project folder and select `Brad_Buchholz.sql` using the file path next to the button.
7. Next click on the `New` button in the section marked `"Default Schema to be imported to"` directly underneath the import options section.
8. Click on the **`Import Progress`** tab at the top of the data import window. At the bottom of this tab click the button that reads **`Start Import`**.
9. Confirm the database has been imported and you can check it by clicking the `Schemas` tab on on the left side of **MySQL Workbench**. Right click the white space and slect **`Refresh All`**.
10. Use your terminal to navigate into the `HairSalon/HairSalon/` fold and use the command **`dotnet run`** to launch the program. The site should be available at the server address used in the `appsettings.json` folder.  

## Known Bugs 
* Application currently has bare bones UI, if I had more time it could use custom styling. 
## License
_Copyright (c) Brad Buchholz_