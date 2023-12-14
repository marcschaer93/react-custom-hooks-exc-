# React Cards

This exercise focuses on writing custom hooks in React. The provided app requires some refactoring.

## Step One: Read the Code

Download and set up the app. It utilizes two APIs (Deck of Cards and Pokemon) to generate different cards on the page. Understand the component hierarchy and how the code functions.

## Step Two: useFlip

Create a `hooks.js` file and write a custom hook called `useFlip`. This hook should manage the flip state of cards and return an array with the current flip state and a function to toggle it. Refactor `PokemonCard` and `PlayingCard` to use this hook.

## Step Three: useAxios in PlayingCardList

Refactor the `PlayingCardList` component to use the `useAxios` custom hook. `useAxios` should handle AJAX requests by accepting a URL and returning an array of data from the requests along with a function to add new data.

## Step Four: useAxios in PokeDex

Modify `useAxios` to accept a base URL and provide flexibility for adding to the response data array in state. Refactor `PokeDex` to utilize this updated `useAxios`. Ensure that `PlayingCardList` continues to function correctly.

## Further Study: Removing response data

Add buttons to erase all playing cards or all Pokemon cards from state. Update `useAxios` to include a function to remove all data from the array in state.

## Further Study: Minimizing state

Implement formatting functions for playing cards and Pokemon cards. Refactor `useAxios` to accept these formatting functions. The arrays in state for `PlayingCardList` and `PokeDex` should only contain necessary data.

## Further Study: useLocalStorage hook

Create a `useLocalStorage` hook that syncs state data with local storage. Refactor `useAxios` to use `useLocalStorage` instead of `useState` to persist cards even after a page refresh.

Show your progress at this stage!
