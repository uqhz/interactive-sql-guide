# Interactive SQL Guide (University data example)

An interactive single-page web application designed as a presentation aid and learning tool for teaching data literacy and foundational SQL concepts. This guide is specifically tailored for a professional development setting within a university, targeting a mixed audience of managers, administrators, and non-technical staff.

**[➡️ View the Live Demo](https://uqhz.github.io/interactive-sql-guide/)**

## Project Overview

The primary goal of this application is not to create expert SQL coders, but to foster **data literacy**. It's built to support a strategic "Why -\> What -\> How" presentation, helping the audience understand the value of data, see what's possible with SQL, and learn how to formulate better data-driven questions.

The entire application is a single `index.html` file, requiring no backend or database setup, making it highly portable and reliable for live presentations.

## Features

  * **Narrative-Driven Content:** The guide is structured as a presentation, moving from the strategic "Why" to a "Guided Tour" of SQL capabilities, and finally to the practical "How."
  * **University-Themed Dataset:** Includes a realistic, multi-table sample database (simulated in JavaScript) with `Courses`, `Lecturers`, and `Enrolments` tables, making the examples immediately relevant to the target audience.
  * **Interactive SQL Widgets:** Each concept in the guided tour is paired with a "Live Demo" area where the presenter can run SQL queries and display results instantly in the browser.
  * **Live Database Explorer:** A dedicated "playground" page that displays the full sample tables and allows for free-form querying, perfect for answering audience questions live.
  * **Conceptual "Slide" Pages:** Includes non-interactive pages that function like presentation slides to explain key strategic concepts like "Database vs. Spreadsheet," "SQL vs. Excel," and the "Anatomy of a Good Data Question."
  * **Responsive Design:** A clean and modern interface built with Tailwind CSS that works on desktops, tablets, and mobile devices.
  * **Zero-Setup Environment:** The entire tool is self-contained in a single HTML file and runs in any modern web browser without needing a server or any installation.

## How to Use

### For Presenting a Session

1.  Open the `index.html` file (or the live GitHub Pages URL) in a web browser.
2.  Use the sidebar navigation to progress through the presentation:
      * Start with **The "Why"** sections to set the strategic context.
      * Move to **The "What"** sections to conduct the live, guided tour of SQL concepts using the interactive widgets.
      * Use the **Live Database Explorer** to answer "what if" questions from the audience in real-time.
      * Conclude with **The "How"** sections to discuss the practical takeaways and benefits for the audience.

### For Local Use or Development

1.  Clone or download the repository.
2.  Open the `index.html` file directly in your preferred web browser. All functionality is client-side and will work locally.

## Technical Details

  * **Frontend:** The application is built with HTML, styled with **Tailwind CSS** (loaded via CDN), and made interactive with **Vanilla JavaScript**.
  * **Database:** A simulated database is created using JavaScript objects within the `<script>` tag of the `index.html` file. This removes the need for any backend or database server setup.
  * **SQL Parser:** The interactive query functionality is powered by a custom, simplified JavaScript function that parses and executes basic SQL commands (`SELECT`, `FROM`, `WHERE`, `ORDER BY`, `GROUP BY`, etc.). It is designed for educational purposes and is not a full-featured SQL engine.

## Future Enhancements

The application is built to be extensible. Future versions could include:

  * **Enabling AI Features:** The code contains hidden "Explain SQL" and "Suggest a Query" buttons that can be activated by adding a valid Google Gemini API key to the script.
  * **Interactive JOINs:** The JavaScript SQL parser could be expanded to handle multi-table `JOIN` operations within the Live Database Explorer.

-----
