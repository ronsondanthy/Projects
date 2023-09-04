# Poll Application Readme

## Introduction

Welcome to the Poll Application project! This web application is built using Django for the back end and HTML/CSS for the front end. The Poll Application allows administrators to create polls with multiple choices and lets users vote for their preferred choices. It also displays the vote results for each choice to users. The application uses SQLite as the database to store poll data.

## Features

- **Admin Dashboard:** The application provides an admin dashboard where administrators can create, manage, and delete polls and their associated choices.

- **User Voting:** Registered users can vote for their preferred choices in the polls.

- **Results Display:** Users can view the vote results for each choice in the poll after they have cast their vote.

- **SQLite Database:** Poll data, including poll questions, choices, and votes, is stored in an SQLite database.

- **Admin Login:** The admin dashboard is protected by a login system, ensuring only authorized users can create and manage polls.

## Installation

To set up the Poll Application on your local development environment, follow these steps:

1. Clone the repository

2. Navigate to the project directory

3. Create a virtual environment (recommended):
   python -m venv venv

4. Activate the virtual environment:

   - On Windows:
     venv\Scripts\activate
    

   - On macOS and Linux:
     source venv/bin/activate
    

5. Install the project dependencies

6. Apply database migrations:
   python manage.py migrate


7. Create a superuser account for admin access:
   python manage.py createsuperuser
   Follow the prompts to set up an admin username and password.

8. Start the development server:
   python manage.py runserver
   The application will be accessible at `http://localhost:8000/`.

## Usage

### Admin Dashboard

1. Access the admin dashboard by navigating to `http://localhost:8000/admin/` and logging in with the superuser credentials you created earlier.

2. Create Polls:
   - Click on "Polls" and then "Add" to create a new poll.
   - Enter the poll question and add choices for the poll.
   - Save the poll.

3. Manage Polls:
   - On the admin dashboard, you can edit, delete, or view poll details by clicking on the respective poll.

### User Voting

1. Users can access the list of available polls by visiting `http://localhost:8000/`.

2. To vote in a poll, click on the poll's title, select a choice, and click the "Vote" button.

3. After voting, users can view the results of the poll, which displays the total votes for each choice.

## Database

The application uses SQLite as the default database, which is stored in the `db.sqlite3` file in the project directory.

## Configuration

The application's settings can be configured in the `polls/settings.py` file, where you can modify various parameters such as database settings, security settings, and more.


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.


Thank you for using the Poll Application! We hope it serves as a useful tool for managing and conducting polls with ease.
