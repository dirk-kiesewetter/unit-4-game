# Crystal Collector

The goal of **Crystal Collector** is to match, but not exceed the randomly-generated score by clicking on each of the crystal buttons.

Each button has a randomly-generated value between 1 and 12.

If the user matches the computer's score, they win, but if they exceed the score, they lose. The random button values and the score to match are regenerated after each win or loss.

This game was coded by me, and is maintained by me.

The deployed app can be found at https://dirk-kiesewetter.github.io/unit-4-game/

---

**Technical details:**

**Problems:** This game needed random numbers for each button, as well as the score to match, that regenerate with each win or loss. A mechanism was also needed to collect each user input on one of the buttons, and add that to the total score. Lastly, some logic was needed to determine when user matches or exceeds the total score, resulting in a win/loss.

**Solutions:**

- The random numbers were generated by a function that used the Math.floor & Math.random functions, with the required minimum & maximum numbers passed as arguments.
- User input was collected via jQuery onclick events individually for each button. Each click of a button runs a function that determines if user has met or exceeded the score to match. If that is the case, another function is run that increments the relevant counter, and resets all the necessary variables.

**Technical Details:**

- The Math.floor & Math.random functions were used in a function to generate the random numbers needed.
- jQuery was used to populate & update the onscreen displays with each user click.
