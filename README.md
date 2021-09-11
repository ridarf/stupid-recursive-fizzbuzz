# Stupid Fizzbuzz Solution

Someone in the web development community asked me if I could make a recursive, one-line solution to the FizzBuzz problem.

What somebody should have asked, is should I. 

The answer is no. *I should not have.*

```js
const recursiveFizzBuzz = (number, output = "", divisor = 1, segments = ["Fizz", "Buzz"]) => (divisor += 2) > 5 ? output || number : recursiveFizzBuzz(number, !(number % divisor) ? (output += segments[(divisor - 1) / 2 - 1]) : output, divisor, segments);
```

One line of code to make any recruiter cry on the spot.
