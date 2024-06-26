# Airbnb Experience Page

This repository houses a React application replicating a simplified version of the Airbnb Experiences page. It demonstrates the core functionalities of building a web interface with React, including:

- **Component-Based Architecture:** The code is organized into reusable components: `Navbar`, `Hero`, and `Card`. This fosters maintainability and scalability.
- **Data Management:** The application utilizes a separate data.js file to store the experience card data, separating data from presentation logic.
- **Conditional Rendering:** The App.js component maps through the data array to dynamically generate individual Card components.
- **Styling:** Basic CSS styles are defined in App.css to provide a clean and visually appealing layout.

## Getting Started

1. **Clone the Repository:** Use git clone `https://github.com/dharm-upenn/React-Projects/Airbnb-Experience-Page.git` to clone this repository.
2. **Install Dependencies:** Navigate to the project directory and run npm install to install required dependencies.

## Project Structure
airbnb-experience-clone/
  - App.css
  - App.js
  - Components/
    - Card.js
    - Hero.js 
    - Navbar.js
   - data.js
   - package.json

## Components:

- **App.js:** The main application component that renders the `Navbar`, `Hero`, and `Card` components.
- **Components/:** A directory containing reusable component files:
  - `Navbar.js:` Renders a simple navigation bar with the Airbnb logo.
  - `Hero.js:` Renders a hero section with an image, header, and descriptive text.
  - `Card.js:` Renders an individual experience card displaying an image, title, price, location, rating, and review count.
- **data.js:** An external JavaScript file that stores an array of experience data objects used to populate the `Card` components dynamically.

## Understanding the Code:

**App.js:**

- Imports necessary components and data.
- Defines a `cards` array by mapping through the `data` array and creating `Card` components for each item.
- Renders the `Navbar`, `Hero`, and `cards` within a main container.

**Components/ (Individual Component Files):**

- Each component imports the `React` library.
- Defines a function component that returns JSX elements representing the component's UI structure.
- Uses props to allow customization of the components' appearance and behavior (e.g., `Card` receives `item` prop for data).

**App.css:**

- Defines basic styles for common elements using CSS selectors.
- Includes styles for fonts, box-sizing, navigation bar, hero section, and card layout.

**To Run the Application:**

1. Start a development server using `npm start`.
2. The application will typically run on `http://localhost:3000/` by default (depending on your development server configuration).

## Customization and Further Development

This project serves as a foundation for building a more elaborate Airbnb Experiences clone. Feel free to explore the following areas for enhancement:

- **Data Fetching:** Implement API integration to fetch real-time experience data from an Airbnb API (if available).
- **Advanced Styling:** Apply more complex CSS techniques for a more polished look and feel.
- **Interactive Features:** Add interactive elements like filtering, sorting, and user interaction with cards.
- **State Management:** Explore state management libraries like Redux or Context API to manage complex application state.
