# DjoserAuth - Django REST Framework Complete Authentication API with Djoser
This repository contains a Django project called "DjoserAuth" that provides a complete authentication API using Django REST Framework and Djoser. The API allows users to register, activate their accounts, login, update their user details, change passwords, and perform other authentication-related tasks.

## Postman Collection
Included in this repository is a file named "DjoserAuth.postman_collection" which contains a Postman Collection. You can import this file into your Postman application to test the API endpoints and explore the authentication functionalities.

## Project Specifications:

Database: The project uses MySQL as the database to store user-related information and authentication data.

Custom User Model: A custom user model is implemented to extend the default user model provided by Django. This allows for additional fields and functionalities tailored to the project's specific requirements.

Custom User Serializer: A custom user serializer is created to control how user data is serialized and deserialized for API interactions. This ensures that only relevant user information is exposed and transmitted securely.

Custom User Model Admin: The Django admin interface is customized to accommodate the extended user model. This allows administrators to manage user accounts efficiently from the backend.

URLs Configuration: The project sets up URL patterns to define API endpoints for user registration, account activation, user details retrieval, login, token generation, user detail updates, password change, password reset request, password reset, and account deletion.

SIMPLE_JWT Settings: The project configures the Simple JWT package to enable JSON Web Token-based authentication, providing secure and efficient access control for the API.

MySQL Client Installation and Database Migration: The mysqlclient library is installed and used to facilitate communication with the MySQL database. The project also performs database migrations to create necessary tables and schema changes.

Email Configuration: Email settings are configured to enable functionalities like account activation and password reset emails to be sent to users securely.

Registration Functionality: Users can register by providing required details, and their accounts are stored in the database for future access.

Account Activation Functionality: Registered users receive an activation link via email to verify and activate their accounts before gaining access to the application.

Retrieving User Details: Authenticated users can retrieve their account details, allowing them to view and update their profile information.

Generating a New Access Token: Users can request a new access token using their refresh token, ensuring continued access to protected resources.

Updating User Details: Authenticated users have the capability to update their account details, such as name, email, or profile picture.

Changing Password: Users can change their passwords securely, providing an extra layer of account protection.

Sending Email to Reset Password: Users can request a password reset via email if they forget their password or suspect unauthorized access.

Resetting Password: Users can securely reset their password using a password reset link sent via email after completing the verification process.

Deleting Account: Authenticated users have the option to delete their accounts, removing their information from the system.

Customizing Email Template: The email templates for account activation and password reset are customized to match the project's branding and improve user experience.


##### Please note that this repository serves as a learning resource and may not be production-ready or actively maintained. Feel free to use it as a reference or starting point for your own authentication-related projects.

### How to Use
To use this project, follow the steps below:

Clone this repository to your local machine using git clone <repository-url>.

Set up a virtual environment and activate it.

Install the required dependencies by running pip install -r requirements.txt.

Configure your database settings in the Django settings file.

Run database migrations using python manage.py migrate.

Start the development server with python manage.py runserver.

You can then interact with the API endpoints using the included Postman Collection or by integrating it into your frontend or mobile applications.




