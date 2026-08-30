# Assignment 1: Getting Your Feet Wet in C

A short first assignment to get you compiling, running, and submitting C. You'll
use variables and types, a **loop**, and **if/else**. Write everything inside
`main` — **do not create your own functions** for this assignment.

Edit **`numbers.c`** and complete the two parts marked `TODO`.

## What to do

**Part A — sizes of types.** Using `sizeof` and the `%zu` format, print the size
in bytes of an `int` and a `double`, each on its own line, exactly in this form
(the numbers come from `sizeof`, don't type them in yourself):

```
int size: 4
double size: 8
```

**Part B — a labeled count from 1 to 10.** Using a **loop**, print the numbers 1
through 10, one per line. For each number, use **if/else** to label it `even` or
`odd`. The output looks like this:

```
1 odd
2 even
3 odd
...
10 even
```

Your program should print Part A first, then Part B.

## Compile and run

In the VS Code terminal (inside the dev container):

```
gcc -Wall numbers.c -o numbers
./numbers
```

`-Wall` turns on warnings — read and fix any that appear. No output from `gcc`
means it compiled.

## Submit

Save and submit with Git each time you make progress:

```
git add .
git commit -m "describe what you did"
git push
```

Your work is checked automatically each time you push. The check is **advisory** —
it gives you fast feedback, but your grade comes from your instructor's review.

## How the check scores you

| Part | Points |
|------|--------|
| Program compiles | 2 |
| Part A: `int size` line | 1 |
| Part A: `double size` line | 1 |
| Part B: all ten labeled lines correct | 6 |

You get partial credit — finishing one part earns those points even if the other
isn't done yet.

## Tips

- The `%zu` format specifier is the correct one for a `sizeof` value.
- A number is even when `n % 2 == 0` (the remainder after dividing by 2 is zero).
- Match the output format exactly — `1 odd`, with a single space, lowercase.
