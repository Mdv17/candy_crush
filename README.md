# About The Project
### The project is a game similar to Candy Crush. 

Everything is implemented in App.jsx. App.jsx is a React functional component that implements a game board with candy-colored squares. It uses useState and useEffect hooks to manage the state of the game board and handle user interactions such as dragging and dropping squares. The component also checks for matches of three or four squares in a row or column and updates the score accordingly.

## Example Usage
```javascript
import React from "react";
import ReactDOM from "react-dom";
import App from "./App";

ReactDOM.render(<App />, document.getElementById("root"));
```

## Code Analysis
### Inputs
- None
___
### Flow
1. The component initializes the state variables `currentColorArrangement`, `squareBeingDragged`, `squareBeingReplaced`, and `scoreDisplay` using the useState hook.
2. The component defines several helper functions to check for matches of three or four squares in a row or column.
3. The component defines the `dragStart`, `dragDrop`, and `dragEnd` functions to handle the dragging and dropping of squares.
4. The component defines the `createBoard` function to randomly generate the initial arrangement of candy-colored squares.
5. The component uses the useEffect hook to call the `createBoard` function once when the component is first rendered.
6. The component uses the useEffect hook to check for matches and update the game board every 100 milliseconds.
7. The component renders the game board using the `currentColorArrangement` state variable and handles user interactions using the defined functions.
8. The component renders the score board using the `scoreDisplay` state variable.
___
### Outputs
- The rendered game board with candy-colored squares that can be dragged and dropped.
- The score displayed on the score board, which is updated based on matches of three or four squares.
___

