# IER Seminar Pizza Calculator

Works out how many Cheese, Pepperoni and Veggie pizzas to order for an IER seminar from the RSVP count.

**Live:** https://linpan498.github.io/pizza-calculator/

## How it counts

1. People = RSVPs + buffer. The speaker buttons set the buffer to +15 (IER speaker) or +20 (external speaker); the slider fine-tunes it.
2. Slices needed = people × 2.25 slices per person (about 0.28 of a pizza each, based on past seminar orders).
3. Pizzas = slices ÷ 8 slices per pizza, rounded up.
4. The pizzas are split by the mix (default 40 / 40 / 20), one at a time, each going to the flavor furthest below its share. Ties go to Cheese, then Pepperoni.

Slices per person, slices per pizza and the mix can all be changed on the page. Changes are saved in the viewer's own browser.

The whole tool is a single `index.html` with no build step.
