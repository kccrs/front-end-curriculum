---
title: Number Guesser
---

Today, you'll be building a game where the user picks a number between 1 and 100.

## Phase One: Basic Requirements

The application should have the following user interface components:

- An input field for guessing the number
- A button for submitting a guess
- A button for clearing the input field
- A button that resets the game to its initial state
- An element that displays the users most recent guess
- An element that displays a message to user
  - If their guess is too high, it should display: "That is too high"
  - If their guess is too low, it should display: "That is too low"

Some things to think about:

- Input fields—regardless of their "type" attribute—store their values in strings. You'll need to use `parseInt()` to turn it back into a number.
- You'll need a strategy for [generating random numbers][rand].

[rand]: http://frontend.turing.io/independent-study/random-numbers.html

## Phase Two: More Better

- The type attribute for the guess input should be "number".
  - It should have "min" and a "max" attributes equal to the minimum and maximum of the reange of guesses (e.g. 1 and 100, respectively).
- The application should display an error message if the guess is not a number (e.g. `parseInt()` returns `NaN`).
  - This may require your input to have two "type" attributes.
- The application should display an error if the guess is outside of the range of possible answers.
- The clear button should be disabled if there is nothing to clear.
- The reset button should be disabled if there is nothing to reset.

## Phase Three: Level Up

- Add additional inputs that allows the user to specify what the minimum and maximum numbers should be.
- Every time the user wins a round increase the maximum number by 10.
- Every time the user wins a round decrease the minimum number by 10.

(**Pro-tip**: You'll need to adjust the input fields to accept the new minimum and maximum numbers.)

#### Layout comps

Desktop layout:

![Number Guesser Desktop][desktop-base]

Mobile layout:

![Number Guesser Mobile][mobile-base]

Color and font spec:

![Design Specs][design-specs]


[desktop-base]: /assets/images/projects/number-guesser/numberguesser1.png
[mobile-base]: /assets/images/projects/number-guesser/numberguesser2.png
[design-specs]: /assets/images/projects/number-guesser/numberguesser3.png

## Rubric

### UX/UI Expectations

- 4: Application matches comp exactly. There are no omitted details. Any extensions are intuitive, well designed, easy to use, and in keeping with the visuals outlined in the comp. Virtually no major improvements are needed in the UX or UI.
- 3: Application shows strong effort towards matching the comp, but some details have been missed. Any extensions are simple, clean design, content organization, and well thought out experience and user interactions.
- 2: Application meets the basic spirit of the comp but overlooks many details. Extensions show questionable design decisions that negatively impact the overall UX/UI.
- 1: Application does not match the comp, is lacking in basic best practices, and user struggles to understand how to use it.

### Functional Expectations

- 4: Application meets all of the functional expectations in Phase Three
- 3: Application meets all of the functional expectations in Phase Two
- 2: Application meets all of the functional expectations in Phase One
- 1: Application does not meet the requirements in Phase One

### Fundamental JavaScript Style

- 4: Application demonstrates excellent knowledge of JavaScript syntax, style, and refactoring
- 3: Application shows strong effort towards organization, content, and refactoring
- 2: Application runs but the code has long functions, unnecessary or poorly named variables, and needs significant refactoring
- 1: Application generates syntax error or crashes during execution
