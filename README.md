# Task Management and Study Timer System

## Overview of the Project

The Task Management and Study Timer System is a lightweight, command-line interface (CLI) application built using Python. It is designed to help students boost productivity by combining two essential tools: a To-Do List for task organisation and a Study Timer for tracking focused work sessions.

The application runs entirely in the python console, offering a simple menu-driven interface to manage tasks and log study duration without the need for complex software or internet connectivity.

## Features

- **Task Management:**

  -Add Tasks:  Input new tasks to your list.

  -View Tasks: See all pending tasks with an index number.

  -Delete Tasks: Remove completed or unwanted tasks by selecting their number.

- **Productivity Timer:**

  -Start Timer: Begin a tracking session for a specific subject.

  -Stop Timer: End the current session and calculate the duration in minutes.

- **View History: Display a log of all completed study sessions with their respective durations.**

- **User-Friendly Interface: simple numeric menu navigation.**

## Technologies/Tools Used

- Programming Language: Python 3.x

- Standard Libraries: time (for timestamp handling and duration calculation)

- Interface:Command Line / Terminal

## Steps to Install & Run the Project

- **Prerequisites**

Ensure you have Python installed on your system. You can verify this by running the following command in your terminal or command prompt:

python--version


If Python is not installed, download it from python.org.

Installation

Download the Code:

Create a new file on your computer named task_manager.py.

Paste the provided source code into this file.

Navigate to the Directory:

Open your terminal or command prompt.

Use the cdcommand to navigate to the folder where you saved task_manager.py.

cd path/to/your/folder


Running the Application

Execute the script using the Python  interpreter:

python task_manager.py


(Note: On some systems, you may need to use python3 instead of python).

## Instructions for Testing

Once the application is running , you will see the TO-DO LIST MENU. Follow these steps to test the functionality:

Test Adding a Task:

Enter 1 and press Enter.

Type Complete Python Assignment and press Enter.

Expected Result: You should see a confirmation message "Task has been added".

Test Viewing Tasks:

Enter 2 and press Enter.

Expected Result: You should see 1. Complete Python Assignment.

Test the Timer:

Enter 4 to Start Timer.

Enter a subject name (e.g., Physics).

Wait for a few seconds/minutes.

Enter 5 to Stop Timer.

Expected Result: The system should print how many minutes you studied.

Test Session History:

Enter 6 to View Timed Sessions.

Expected Result: You should see an entry for Science with the calculated duration.

Test Deleting a Task:

Enter 3.

Enter the task number 1.

Expected Result: The task should be removed. Verify by pressing 2 (View Tasks) again to see if the list is empty.

Exit:

Enter 7 to close the application.
