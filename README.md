# LLM-Enhanced Learning Assistant

## Overview
LLM-Enhanced Learning Assistant is an Android mobile application built in Java using Android Studio.  
The app is designed to support students by generating short learning activities powered by an LLM.

## Features
- User Registration and Login
  - Users can create an account, log in, and log out.
  - Session state is stored locally using SharedPreferences.

- Interest Selection
  - Users select learning interests such as Algorithms, Data Structures, Cyber Security, and others.
  - These interests are used to generate personalized questions and learning support through the LLM.

- AI-Generated Tasks
  - The app requests a personalized task from the backend.
  - Each generated task contains:
    - a topic
    - a short lesson summary
    - two multiple-choice questions
    - answer options and correct answers

- AI Learning Utilities
  - Generate Hint: provides a hint for the current question.
  - Explain My Answer: explains the selected answer using AI-generated feedback.

- Results Screen
  - After completing both questions, the app displays:
    - Question 1 result
    - Question 2 result
    - an overall summary

- Recent Activity
  - The app stores completed learning interactions locally using Room.
  - The latest activity is shown on the dashboard.

## Built With
- Java
- Android Studio
- XML
- SharedPreferences
- Room Database
- Retrofit
- Gson
- Node.js backend
- Gemini API

## Backend Note
This Android project communicates with a separate backend server using Retrofit. The backend is responsible for:
- receiving task generation and learning feedback requests
- calling the Gemini API
- returning structured JSON responses to the Android app

## How to Run
1. Open the project in Android Studio
2. Sync the Gradle files
3. Run the app using an emulator or Android device

## Backend
This app expects a backend running locally at `http://10.0.2.2:3000/`

## Future Changes
- Replace the current local account system with proper Room-based user storage
- Refactor the task structure into a more object-oriented design for easier expansion and maintenance

## Author
Dean Kennedy  
s224318581
