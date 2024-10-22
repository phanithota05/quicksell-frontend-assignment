# Interactive Kanban Board with React JS

## Overview

This project is a **Kanban board application** built using **React JS**. It allows users to group and sort tasks (or tickets) based on various criteria. The UI mimics a traditional Kanban board, and the data is dynamically fetched from an API. This project is designed to be lightweight and functional without using external CSS libraries, relying instead on **pure CSS** for styling.

## Features

- **Dynamic Grouping**:
  - **By Status**: Group tasks based on their status.
  - **By User**: Organize tasks by the assigned user.
  - **By Priority**: Group tasks by priority levels, ranging from "Urgent" to "No Priority".

- **Sorting Options**:
  - **By Priority**: Sort tasks in descending order based on priority.
  - **By Title**: Sort tasks alphabetically by title.

- **Persistent State**: The application saves user preferences (such as grouping and sorting selections) and maintains them even after the page reloads.

- **Responsive UI**: The Kanban board is fully responsive, adapting to various screen sizes while maintaining usability and design consistency.

## API Integration

The Kanban board fetches task data from the following API endpoint:
**https://api.quicksell.co/v1/internal/frontend-assignment**

This API provides all the ticket information necessary for the board to function.
The API returns ticket information, which is then grouped and displayed on the board according to the user's preferences.

## Priority Levels

The API returns tickets with the following priority levels:

| Priority Level | Description   |
|----------------|---------------|
| 4              | Urgent        |
| 3              | High          |
| 2              | Medium        |
| 1              | Low           |
| 0              | No Priority   |

## Installation

To run the project locally, follow these steps:

1. Clone the repository:
   -> git clone https://github.com/phanithota05/quicksell-frontend-assignment.git

2. Navigate to the project directory:
  cd quicksell-frontend-assignment

3.Install the dependencies:
  npm install

4.Start the development server:
  npm start
  Open your browser and go to http://localhost:3000.

5.Project Structure
The project is structured as follows:
/src
  /components
    - KanbanBoard.js      // Main Kanban board component
    - TicketCard.js       // Component for individual ticket display
    - Header.js           // Header and control elements (grouping/sorting)
  /styles
    - kanbanBoard.css     // Styles for the Kanban board layout
    - ticketCard.css      // Styles for the ticket card component
  - App.js                // Entry point of the application
  - index.js              // Main render file

6.Technologies Used
React JS: Used for building the interactive user interface.
Pure CSS: Custom styles for layout and design without using CSS frameworks.
Styled JSX: For component-specific styles.
JavaScript ES6: Core language for building logic and functionality.

