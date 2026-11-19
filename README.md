# Toggle Message App

A simple React application component that demonstrates conditional
rendering and state management using the `useState` Hook. Users can
click a button to show or hide a message.

## Features

-   **Show/Hide toggle:** Click the button to display or hide the
    message.
-   **Dynamic button label:** The button changes between **Show
    Message** and **Hide Message** based on the current visibility
    state.
-   **Conditional rendering:** The message is rendered only when it is
    visible.
-   **React state management:** Uses the `useState` Hook to track
    visibility.

## Technologies Used

-   React
-   JavaScript (JSX)
-   HTML elements styled through CSS selectors

## Project Structure

``` text
project/
├── src/
│   └── ToggleApp.jsx
└── README.md
```

The structure above is a suggested placement for the component; the
uploaded source contains `ToggleApp.jsx`.

## How It Works

1.  The component initializes `isVisible` to `false`, so the message is
    hidden when the app first loads.
2.  Clicking the button calls `handleToggleVisibility`.
3.  The handler updates the state by switching `isVisible` to its
    opposite value.
4.  The button label updates automatically:
    -   When the message is hidden, it displays **Show Message**.
    -   When the message is visible, it displays **Hide Message**.
5.  React conditionally displays the paragraph `I love Computer!` when
    `isVisible` is `true`.

## Getting Started

### Prerequisites

-   Node.js and npm
-   A React project (for example, one created with Vite)

### Setup

1.  Open your React project.
2.  Place `ToggleApp.jsx` inside the `src` directory.
3.  Import and render the component in your app's entry component, such
    as `App.jsx`:

``` jsx
import { ToggleApp } from "./ToggleApp";

function App() {
  return <ToggleApp />;
}

export default App;
```

4.  Start the development server using the command provided by your
    React project. In a typical Vite project, run:

``` bash
npm install
npm run dev
```

## CSS Customization

The component includes these element IDs, which you can target in your
CSS:

-   `#toggle-container` --- the main container
-   `#toggle-button` --- the toggle button
-   `#message` --- the message paragraph

No CSS styling is included in the uploaded component, so you can add
your own styles.

## Learning Outcomes

This exercise demonstrates how to:

-   Declare and update state with React's `useState` Hook.
-   Handle button click events with `onClick`.
-   Use conditional rendering with the logical `&&` operator.
-   Update interface text dynamically based on component state.

## Notes

-   The message is hidden by default.
-   The component manages its own visibility state.
-   The uploaded source does not include styling, tests, or a complete
    React project configuration.

## Author

Add your name here.
