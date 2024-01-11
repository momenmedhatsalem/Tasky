# Tasky - Professional Readme

## Overview

Welcome to Tasky, a web application designed to streamline your task management and enhance productivity. This readme provides a comprehensive guide to Tasky's features and functionalities.

### Video Demo

Watch a detailed demonstration of Tasky [here](https://youtu.be/che_1sVpy9g).

## Description

Tasky offers a user-friendly interface for organizing tasks and collaborating with friends. Key features include:

1. **User Management:** Users can log in and out of their accounts, ensuring secure access to Tasky.

2. **Task Organization:** Tasks are sorted by time and day, providing a clear overview of upcoming and completed activities.

3. **Task Creation:** Users can add tasks with detailed information, including the date, description, and time.

4. **Task Completion:** Completed tasks can be checked off, automatically transferring them to the completed tasks list.

5. **Task Deletion:** Users have the ability to delete tasks by clicking the trash can icon next to each task.

6. **Friend Collaboration:** Tasky allows users to add friends, providing visibility into each other's finished and unfinished tasks.

7. **Password Change:** Users can update their passwords by entering the old password and then setting a new one. The system verifies the old password before allowing the update.

8. **Privacy Settings:** Users can control whether friends can view their tasks by toggling a privacy setting in the account section.

## Database Structure

Tasky employs an SQL database with three tables:

1. **Users Table:** Contains user information, including username, ID, number of friends, and a binary value indicating whether friends can view tasks (0 for not allowing, 1 for allowing).

2. **Friends Table:** Tracks added friends and is updated each time a user adds a new friend.

3. **Tasks Table:** Organizes tasks with fields for name, description, date, time, and a link to the user. Deleting a task removes the corresponding row from the SQL tasks table.

## Usage Guidelines

1. **Adding Friends:** Users can add friends by searching for their usernames. Duplicate friend requests are not permitted.

2. **Error Handling:** Attempts to look up oneself or a name not in the database will result in an error message.

3. **Task Completion:** Completed tasks can be viewed in the completed tasks section.

4. **Privacy Control:** Users can enable or disable friends' visibility into their tasks via the account section.

Please note that friends must grant permission for their tasks to be visible. If a friend disables this feature, tasks will remain private.

Thank you for using Tasky! We hope it enhances your task management experience.
