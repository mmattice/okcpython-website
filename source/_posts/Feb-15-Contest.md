layout: post
title: "Feb '15 Contest"
date: 2015-02-11 12:30:00
post_asset_folder: true
tags: [Contest]
categories: [Contest]
---

# Numbers Game

One of the longest-running quiz shows on UK TV is called Countdown, and has a "numbers round". There are some cards laid face down in front of the host - the top row contains 'large' numbers (from the set 25, 50, 75, 100), and the rest are 'small' (1 to 10). Six cards are picked and displayed: the choice is made by one of the contestants, who typically will ask for one large number and five small ones.

Next, a machine called "Cecil" picks a target number between 100 and 999 at random. The contestants then have 30 seconds to find a way of combining the source numbers using the normal arithmetic operators (+, -, *, /) to make the target number, or to get as close as possible.

Each source number can be used 0 or 1 times.

### Easy Example

    source 50 9 4 1 10 2
    target 402

    ( 50 * (9 - 1) ) + 2 = 402
    -- OR --
    ( ( ( 50 * 10 ) / 4 ) + 9 ) * ( 2 + 1 ) = 402

### Medium Example
    source 100 5 5 2 6 8
    target 522

    100 *  5 = 500
      5 +  6 =  11
     11 *  2 =  22
    500 + 22 = 522

Resulting in `(5*100)+((5+6)*2) = 522`

Another solution is `(100+6)*5-8 = 522`

### Hard Example
    source 75 5 4 4 9 7
    target 933

       9 * 7  = 63
      63 * 4  = 252
     252 * 4  = 1008
    1008 - 75 = 933

Resulting in `((9 * 7 * 4) * 4) - 75 = 933`

Another solution is `( ( (9 * 7) * ( (5 * 4) - 4 ) ) - 75 = 933`

----------------

Normal arithmetic rules apply, and in particular you are not allowed to use integer rounding. That is, 7 divided by 3 is 2 1/3, not 2.

The program will accept one target number and a list of source numbers, and generate a solution which calculates the target or a number as close to the target as possible. Solve for the 3 examples above. You can consult http://www.crosswordtools.com/numbers-game/ for more games and solutions if you need more for testing.

# Execution

**NOTE: lines starting with `$` signify a command prompt line, and lines starting with `>` signify output from the executed program.**

Assuming your main python file is named `numbers_game.py`, then to execute we would call:

    $ python numbers_game.py target num1 num2 num3 ... numN
    > (mathematical formula)

for example:

    $ # medium example above
    $ python numbers_game.py 522 100 5 5 2 6 8
    > (100 + 6) * 5 - 8 = 522

Whitespace in output is optional.

# Judging

The results will be judged primarily on correctness, then succinctness of solution.  Solutions that take longer than a second to execute will be penalized relative to other correct solutions.