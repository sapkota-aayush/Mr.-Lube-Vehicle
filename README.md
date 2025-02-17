Mr. Lube Vehicle Management Software
Overview
This project is an imitation of the Mr. Lube Automotive Repairing Software, inspired by my past work as a technician at Mr. Lube. The software is built using C++ and MySQL, with a strong emphasis on Object-Oriented Programming (OOP) principles.

Key Features
✅ Add vehicle information and check if it exists in the database.
✅ Retrieve previous service history.
✅ Perform new services and update the database.
✅ Process payments and view payment history.
✅ Send receipts to customers via email using the SendGrid API.
✅ Secure authentication system for users.
✅ Uses cURL for HTTP requests and nlohmann/json for JSON handling.
✅ Graphical User Interface (GUI) built with Qt for an enhanced user experience.
Project Structure
The project consists of 11 files: 5 header files and their corresponding 5 implementation files, along with main.cpp as the entry point.

Header Files (.h)
authsystem.h - Handles authentication.
services.h - Manages vehicle services.
payment.h - Handles payment transactions.
utility.h - Contains utility functions (e.g., validation).
vehicle.h - Manages vehicle data and service history.
Source Files (.cpp)
authsystem.cpp - Implements authentication logic.
services.cpp - Implements service functionalities.
payment.cpp - Implements payment processing.
utility.cpp - Implements utility/helper functions.
vehicle.cpp - Implements vehicle management.
main.cpp - The main entry point that ties everything together.
Installation Guide
To set up this project, follow these steps:

1. Install MySQL and Configure Database
Follow this guide to set up MySQL in Visual Studio for a C++ application:
MySQL Setup Guide

2. Install Required Libraries
nlohmann/json (for JSON parsing)
Install the nlohmann/json library via vcpkg:

sh
Copy
Edit
vcpkg install nlohmann-json
Or download it manually from the nlohmann/json GitHub repository.

cURL (for HTTP requests - Sending emails via API)
Install cURL on Windows:

sh
Copy
Edit
vcpkg install curl
Link cURL to your C++ project in Visual Studio:

Go to Project Properties > C/C++ > Additional Include Directories
Add the path to cURL's include directory.
Qt (for GUI development)
Download and install Qt from the Qt Official Site.
Configure Qt in your development environment:
Add Qt include and library paths to your project settings.
Ensure the correct Qt version is selected in your IDE.
Usage
Authentication - Log in to the system.
Vehicle Lookup - Enter vehicle details to check service history.
Service Addition - Add new services to the selected vehicle.
Payment Processing - Handle payments and generate receipts.
Email Receipt - Send a receipt to the customer via the SendGrid API.
User Interface - Perform all operations using the Qt-based GUI.
API Configuration (SendGrid for Email)
Sign up at SendGrid.
Generate an API key.
Store the key in an environment variable or a config file.
Screenshots / Demonstrations
Due to some Visual Studio Code 2022 issues, I have not pushed the code yet. However, you can view the screenshots and demonstrations of the software via this Google Drive folder.

Why This Project?
This project is a practical demonstration of how OOP (Object-Oriented Programming) simplifies software design and maintenance by abstracting underlying complexity. It mimics real-world software used in the automotive industry to manage vehicle services efficiently.

Future Enhancements
Expand GUI features with more interactive elements.
Implement multi-user authentication roles (e.g., Admin, Technician).
Improve error handling and logging.
Expand email templates for better customer communication.
Reference Project
For additional inspiration, check out this Insurance Management system:
Insurance Management on GitHub

Contributor
👨‍💻 Aayush Sapkota

💡 Feel free to contribute, suggest improvements, or fork this repository! 🚀

