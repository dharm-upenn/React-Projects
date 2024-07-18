# Meme Generator

This React application lets you create custom memes by overlaying text on a variety of meme images. It demonstrates several key React concepts you'll encounter while building modern web interfaces:

- **Component-Based Architecture:** The code is structured into reusable components for maintainability and scalability:
  - `Header` displays the project title and logo.
  - `Meme` handles the meme generation logic, user input, and image display.
- **Data Fetching and Management:** The `Meme` component fetches meme data (image URLs) from an API (https://api.imgflip.com/get_memes) and updates the application state using `useState` and `useEffect`.
- **State Management with Hooks:** The `useState` hook manages the application state, including:
  - `meme` object: Stores the top and bottom text, and the currently displayed meme image URL.
  - `allMemes` array: Holds the fetched meme data (image URLs) from the API.
- **Event Handling:** The `handleChange` function handles user input from the text fields, updating the `meme.topText` and `meme.bottomText` state.
- **Conditional Rendering:** The `randomImage` in the `Meme` component is conditionally updated with a new image URL based on user interaction.
- **Basic Styling with CSS:** The `App.css` file provides basic styling for the layout and visual elements.

## Getting Started

1. **Clone the Repository:** Use git clone `https://github.com/dharm-upenn/React-Projects/Meme-Generator.git` to clone this repository.
2. **Install Dependencies:** Navigate to the project directory and run `npm install` to install required dependencies.

## Project Structure
meme-generator/
  - App.css
  - App.js
  - Components/
    - Header.js
    - Meme.js 
   - package.json

## Components:

- **App.js:** The main application component that renders the `Header` and `Meme` components.
- **Components/:** A directory containing reusable component files:
  - `Header.js`: Renders a header displaying the project title, logo, and some project context.
  - `Meme.js`: Manages the meme generation experience:
    - Fetches meme data (image URLs) using `useEffect` on component mount.
    - Handles user input for top and bottom text using `handleChange` and updates the `meme` state.
    - Generates a random meme by selecting an image URL from `allMemes` and updates the `meme.randomImage` state.
    - Renders the meme image and text input fields.

## Understanding the Code:

**App.js:**

- Imports necessary components and data.
- Renders the `Header` and `Meme` within a main container.

**Components/ (Individual Component Files):**

- Each component imports the `React` library.
- Defines a function component that returns JSX elements representing the component's UI structure.
- Uses props where applicable to customize appearance and behavior (e.g., `Header` could accept a title prop).

**App.css:**

- Defines basic styles for common elements using CSS selectors.
- Includes styles for fonts, box-sizing, layou, and visual elements as needed

**To Run the Application:**

1. Start a development server using `npm start`.
2. The application will typically run on `http://localhost:3000/` by default (depending on your development server configuration).

## Customization and Further Development

This project serves as a solid foundation for a more comprehensive meme generator. Here are some areas for exploration:

- **API Integration:** Utilize a more extensive meme API to access a wider variety of images or additional meme data.
- **State Management Library:** Consider using a state management library like Redux or Context API for more complex applications with intricate data flows.
- **Advanced Styling:** Integrate CSS frameworks like Bootstrap or Material-UI for more sophisticated layouts and design patterns.
- **Image Uploading:** Allow users to upload their own images for meme creation.
- **Persistence:** Enable users to save or share their generated memes.


**Feel free to contribute your own ideas to enhance this project!**
