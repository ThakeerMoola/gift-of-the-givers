Gift of the Givers Web Application
Overview
The Gift of the Givers Foundation stands as a beacon of hope in times of crisis, dedicated to providing swift and effective aid to communities struck by natural disasters and emergencies in South Africa and beyond. This project aims to develop a comprehensive C# web application for the foundation, serving as a centralized hub for managing relief efforts, coordinating volunteers, and facilitating resource allocation during times of crisis.

Key Features
Incident Reporting: Users can report incidents related to natural disasters and emergencies, ensuring that the foundation can respond quickly and effectively.
Donation Management: Users can make donations to support the foundation's efforts, helping to fund critical relief initiatives.
Volunteer Coordination: Individuals can sign up to become volunteers, facilitating the mobilization of resources and personnel during crises.
Technologies Used
ASP.NET MVC: For building the web application and implementing the Model-View-Controller design pattern.
Entity Framework: For data access and management, enabling interactions with the database.
Azure SQL Database: For storing user and incident data securely in the cloud.
HTML/CSS/JavaScript: For front-end development, ensuring a responsive and user-friendly interface.
Bootstrap: For responsive design and UI components.
Getting Started
Prerequisites
Visual Studio: Ensure you have Visual Studio installed with the ASP.NET and web development workload.
Azure Account: An active Azure subscription to set up the Azure SQL Database and host the application.
Installation
Clone the Repository:

bash
Copy code
git clone <repository-url>
cd GiftOfTheGiversApp
Open the Project in Visual Studio:

Open the .sln file in Visual Studio.
Install NuGet Packages:

Right-click on the project in Solution Explorer and select Manage NuGet Packages.
Install the required packages:
Entity Framework
Microsoft.AspNet.Identity.Core
Microsoft.AspNet.Identity.EntityFramework
Set Up Database:

Open the Web.config file and update the connection string to your Azure SQL Database.
xml
Copy code
<connectionStrings>
  <add name="DefaultConnection" 
       connectionString="Server=tcp:<your-server>.database.windows.net,1433;Initial Catalog=<your-database>;Persist Security Info=False;User ID=<your-username>;Password=<your-password>;MultipleActiveResultSets=False;Encrypt=True;TrustServerCertificate=False;Connection Timeout=30;" 
       providerName="System.Data.SqlClient" />
</connectionStrings>
Run Migrations:

Open Package Manager Console and run the following commands:
powershell
Copy code
Enable-Migrations
Add-Migration InitialCreate
Update-Database
Build and Run the Application:

Press F5 to build and run the application.
Navigate to the home page to start using the application.
Usage
User Registration: Users can create an account to access the full features of the application.
Report an Incident: Logged-in users can report incidents, which will be stored in the database.
Make a Donation: Users can donate funds to support relief efforts.
Become a Volunteer: Users can apply to volunteer, enabling the foundation to coordinate relief operations effectively.
Contributing
Contributions are welcome! If you would like to contribute to this project, please follow these steps:

Fork the repository.
Create a new branch (git checkout -b feature/YourFeature).
Make your changes and commit them (git commit -m 'Add some feature').
Push to the branch (git push origin feature/YourFeature).
Open a pull request.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
Thanks to the Gift of the Givers Foundation for their inspiring work in disaster relief.
Special thanks to all contributors who help improve this project.