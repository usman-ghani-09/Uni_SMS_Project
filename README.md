Student Management System (C & GTK4)
This is a fast, native desktop app we built to make school management simple. It’s written in C and uses the GTK4 library to create a modern, professional-looking interface that’s easy for anyone to navigate.

## What’s Under the Hood?
We’ve organized the app into different modules so it stays clean and easy to update:

Authentication: A secure Login and Logout system to keep student data private.

Student Manager: The main place to register new students and update their info.

Attendance: A simple digital tracker to log daily presence.

Fees & Billing: A dedicated spot to track tuition payments and see who still has an outstanding balance.

Academic Grades: Separate sections for Exams and Tests so you can manage big finals and quick quizzes differently.

## Getting It Running (MSYS2)
Since we are using MSYS2 on Windows, setting this up is a breeze.

1. Prep your environment
Open your MSYS2 UCRT64 terminal and make sure the GTK4 toolkit is installed:

Bash
pacman -S mingw-w64-ucrt-x86_64-gtk4
2. Build the project
We’ve included a Makefile to save you from typing long commands. Just navigate to the project folder and type:

Bash
make
This will automatically find your files, link the GTK4 libraries, and create your executable file.

3. Start the app
Bash
./sms.exe
## Why We Built It This Way
Fast & Light: By using pure C, the app is incredibly lightweight. It doesn't hog your RAM and starts up instantly.

Modern UI: We built the interface using GTK4, which means the buttons, layouts, and menus look modern and respond smoothly.

Easy to Manage: Thanks to the Makefile and the modular code, adding a new feature or fixing a bug is quick and doesn't turn into a mess.

## How to Use
Login: Enter your credentials to get into the dashboard.

Work: Switch between Students, Fees, or Attendance using the main menu.

Logout: When you're done, log out to return to the secure sign-in screen.
