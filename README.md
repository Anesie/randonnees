# ⛰️ Hiking Management Platform

## 📖 Presentation
This project is a full-stack web application that allows users to record, explore, and rate hiking trails. It was developed as part of the MIASHS Bachelor's degree (Computer Science and Cognition) at Université Grenoble Alpes (UGA).

The application relies on a client-server architecture developed in **Node.js** with an integrated **SQLite** database. It features a secure authentication system and multiple asynchronous interactions (AJAX) to provide a smooth user experience without page reloads.

## ✨ Features
The project integrates all requirements of the Minimum Viable Product (MVP) as well as advanced features:

### 🗺️ Hiking Management
- **Exploration:** Home page listing all hiking trails with their names, starting addresses, and illustration photos.
- **Dynamic Sorting:** Ability to sort hiking trails alphabetically or by popularity score dynamically without reloading the page (AJAX).
- **Details:** Dedicated pages for each hike displaying the full description, starting address, and average rating[cite: 3, 4].
- **Contribution:** Trail creation form (name, description, address, photo upload) that automatically redirects to the newly created trail page.

### 🔐 Authentication & Security
- **User Management:** Unified login and registration form (with a checkbox for new users).
- **Data Security:** Systematic cryptographic password hashing before saving to the database).
- **Access Control:** Automatic redirection to the login page if an unauthenticated user attempts to access the "Contribute" page (route protection).
- **Client-Side Error Handling:** Asynchronous error messaging (incorrect password, non-existent or already taken username) without reloading the page.

### ⭐ Rating System
- **Evaluation:** Logged-in users can rate each hike from 1 to 5 stars.
- **Uniqueness:** Only one rating allowed per user per hike.
- **Smooth Experience:** Asynchronous rating submission with client-side network error handling (e.g., lost server connection).

## 🛠️ Technologies Used
- **Backend:** Node.js (LTS version)
- **Database:** SQLite (Embedded relational database)
- **Frontend:** HTML5, CSS3, JavaScript (Vanilla, Fetch API for AJAX)

## 🚀 Installation and Setup
The application is designed to run independently without installing third-party software (other than Node.js).

1. Clone the repository to your local machine:
   ```bash
   git clone [https://github.com/Anesie/randonnees](https://github.com/Anesie/randonnees) ```

2. Navigate into the project folder:
    ```bash
   cd randonnees
    ```
3. Install project dependencies:
    ```bash
    npm install
    ```
4. Initialize the SQLite database:
    ```bash
   npm run init-db
    ```
5. Start the local server:
    ```bash
   npm run start
    ```
6. Open your browser and access the application on port 8080:
    ```bash
    http://localhost:8080
     ```

### 📋 Code Quality
The project was developed in compliance with web standards (validated via the W3C Validator). Special attention was paid to code indentation, clarity, simplicity, and overall interface ergonomics.   

### 👥 Author
Anesie Martiniani - Development (L3 MIASHS)
