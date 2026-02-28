# Tech Talks Today Event App

This is a single-page web application displaying the schedule for a 1-day technical talks event, "Tech Talks Today". Users can view the full schedule with timings and search for talks based on their categories.

## Features

- **Event Schedule:** Displays 6 technical talks, each 1 hour long, with 10-minute transitions and a 1-hour lunch break.
- **Talk Details:** Each talk includes a title, speaker(s), category keywords, duration, and a description.
- **Search by Category:** Users can filter talks by entering keywords in the search bar.
- **Serverless:** The entire application is contained within a single `index.html` file, making it easy to deploy and host.

## Technologies Used

- HTML
- CSS
- JavaScript

## Setup and Running Locally

To run this application locally, you can use any simple HTTP server. Here's how to do it using Python's built-in HTTP server:

1.  **Clone the repository (if you haven't already):**
    ```bash
    git clone https://github.com/Chawjyoti/Chawjyoti-event-talks-app.git
    cd Chawjyoti-event-talks-app
    ```
2.  **Start a simple Python web server:**
    ```bash
    python3 -m http.server
    ```
    If you don't have Python, you can use other methods like `npx http-server` if you have Node.js installed, or any other static file server.

3.  **Open your web browser:**
    Navigate to `http://localhost:8000` (or the port indicated by your server).

## Project Structure

- `index.html`: Contains all the HTML structure, CSS styling, and JavaScript logic for the application.
- `.gitignore`: Specifies intentionally untracked files that Git should ignore.

## Talks Data

The talk data is embedded directly within the `index.html` file as a JavaScript array of objects. Each talk object has the following properties:

- `title`: The title of the talk.
- `speakers`: An array of speaker names.
- `category`: An array of keywords describing the talk's category.
- `description`: A brief description of the talk.
