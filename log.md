# 100 Days Of Code - Log

### Day 1: December 30, 2017

**Today's Progress**:
Continued to struggle with the Fib challenge on fcc.

**Thoughts**:
Feeling so rusty.

**Link(s) to work**
1. [Sum All Odd Fibonacci Numbers](https://www.freecodecamp.org/challenges/sum-all-odd-fibonacci-numbers)


### Day 2: December 31, 2017

**Today's Progress**:
Continued to struggle with the Fib challenge on fcc. Finally looked at the spoiler. Was on the wrong track with trying recursive.

**Thoughts**:
Was very frustrated. Also was a little rude in front of company logging in late just before midnight and after a few beers. Not the ideal state of mind.

**Link(s) to work**
1. [Sum All Odd Fibonacci Numbers](https://www.freecodecamp.org/challenges/sum-all-odd-fibonacci-numbers)


### Day 3: January 1, 2018

1/1/2018, 10:16:37 PM
On to the next challenge on fcc.

**Today's Progress**:

"Sum All Prime"

The suggestion of 'pair programming' is interesting.
Haven't tried that online.

1/1/2018, 11:13:20 PM

- Played around with Atom and trying setup an environment for pair programming. Floobits and Teletype look like interesting tools I'd like to play with another developer to see if it's actually productive.

- Just started looking at the challenge. Actually looks very similar to the previous challenge.
Found a quick a dirty snippet at first google result:

```
function isPrime(number) {
  if (typeof number !== 'number' || !Number.isInteger(number)) {
    return false;
  }

  if (number < 2) {
    return false;
  }

  if (number === 2) {
    return true;
  } else if (number % 2 === 0) {
    return false;
  }

  for (var i = 3; i*i <= number; i += 2) {
    if (number % i === 0) {
      return false;
    }
  }
  return true;

}

console.log(isPrime(6));
console.log(isPrime(15485863));
```

**Thoughts**:
More playing around with a working environment than actual coding. Not a bad issue but I suspect my "saboteur" is that I love playing with tools and environments than than doing the tough coding challenges. This keeps me from progress and further more from entering that sweet "flow state". That being said learning about setting up a new environment for a remote team in the future is probably a very valuable skill.

**Link(s) to work**
1. [Floobits](https://floobits.com/)
2. [Prime result](https://codepen.io/codepatel/pen/vOqWBe?editors=0011)
