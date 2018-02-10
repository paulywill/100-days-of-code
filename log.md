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

console.log(isPrime(1));
console.log(isPrime(15485863));
```

**Thoughts**:
More playing around with a working environment than actual coding. Not a bad issue but I suspect my "saboteur" is that I love playing with tools and environments than than doing the tough coding challenges. This keeps me from progress and further more from entering that sweet "flow state". That being said learning about setting up a new environment for a remote team in the future is probably a very valuable skill.

**Link(s) to work**
1. [Floobits](https://floobits.com/)
2. [Prime result](https://codepen.io/codepatel/pen/vOqWBe?editors=0011)


### Day 4: January 2, 2018

**Today's Progress**:
This morning I figured out how to finish setting up Atom environment.

A little before lunch received news about a death in the family.... so, mind once again not operating at 100%.

I did continue the fcc problem (working inside Atom). I found several examples to find prime numbers, however none of them explained the code until I came across an article that mentioned Sieve of Eratosthenes' algorithm.

The wikipedia entry does an excellent job explain the solution and even providing Pseudocode.

Example

To find all the prime numbers less than or equal to 30, proceed as follows.

First generate a list of integers from 2 to 30:

 2  3  4  5  6  7  8  9  10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30

The first number in the list is 2; cross out every 2nd number in the list after 2 by counting up from 2 in increments of 2 (these will be all the multiples of 2 in the list):

 2  3  ~~4~~  5  ~~6~~  7  ~~8~~  9  ~~10~~ 11 ~~12~~ 13 ~~14~~ 15 ~~16~~ 17 ~~18~~ 19 ~~20~~ 21 ~~22~~ 23 ~~24~~ 25 ~~26~~ 27 ~~28~~ 29 ~~30~~

The next number in the list after 2 is 3; cross out every 3rd number in the list after 3 by counting up from 3 in increments of 3 (these will be all the multiples of 3 in the list):

 2  3  ~~4~~  5  ~~6~~  7  ~~8~~  ~~9~~  ~~10~~ 11 ~~12~~ 13 ~~14~~ ~~15~~ ~~16~~ 17 ~~18~~ 19 ~~20~~ ~~21~~ ~~22~~ 23 ~~24~~ 25 ~~26~~ ~~27~~ ~~28~~ 29 ~~30~~

The next number not yet crossed out in the list after 3 is 5; cross out every 5th number in the list after 5 by counting up from 5 in increments of 5 (i.e. all the multiples of 5):

 2  3  ~~4~~  5  ~~6~~  7  ~~8~~  ~~9~~  ~~10~~ 11 ~~12~~ 13 ~~14~~ ~~15~~ ~~16~~ 17 ~~18~~ 19 ~~20~~ ~~21~~ ~~22~~ 23 ~~24~~ ~~25~~ ~~26~~ ~~27~~ ~~28~~ 29 ~~30~~

The next number not yet crossed out in the list after 5 is 7; the next step would be to cross out every 7th number in the list after 7, but they are all already crossed out at this point, as these numbers (14, 21, 28) are also multiples of smaller primes because 7 × 7 is greater than 30. The numbers not crossed out at this point in the list are all the prime numbers below 30:

 2  3     5     7           11    13          17    19          23                29


```
Input: an integer n > 1.

 Let A be an array of Boolean values, indexed by integers 2 to n,
 initially all set to true.

 for i = 2, 3, 4, ..., not exceeding √n:
   if A[i] is true:
     for j = i2, i2+i, i2+2i, i2+3i, ..., not exceeding n:
       A[j] := false.

 Output: all i such that A[i] is true.
```


**Thoughts**:

The family emergency through me off my challenge today. Ideally I wanted to finish the challenge today and be done with it, but life had other plans. Though I like that I'm now at the point in fcc where I have to learn what snippets are really doing. This is the first time I've learned about the Sieve of Eratosthenes' algorithm. It's pretty cool. Deep learning now rather than chewing out code.

Tomorrow I hope to land the plane on this one.

My Pseudocode:
```
function sumPrimes(num) {

  //Error handling on num

  //Check num is not a prime

  Sieve of Eratosthenes

  //For loop through to find all primes to num push into Array

  for (loop){
    Sieve of Eratosthenes
    arr.push(primeNum)
  }

  //Reduce array to find the sum

  return sum;
}
```


**Link(s) to work**
1. [Prime Number Explained](https://www.thepolyglotdeveloper.com/2015/04/determine-if-a-number-is-prime-using-javascript/)
2. [Sieve of Eratosthenes' algorithm](https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes)


### Day 5: January 3, 2018
**Today's Progress**:
Took a small break from the fcc's challenges and worked on investigating an issue on fcc's League for Good.

Which lead to spending some time setting up lfg project on a c9 environment on my aws so I could do some work and testing on it at work.

I did have to change the default port form 4000 to 8080 as a work around.

I'm hoping there's a way to change it back to 4000 or find a way to ensure it will not be added to a future PR.

**Thoughts**:
I find the 100DaysOfCode challenging as I tend to switch between coding and setting up infrastructure to test code. As long as I'm working and learning on something everyday I still think it's a win.

ˇ
**Link(s) to work**

1. [League-For-Good Issue 73](https://github.com/freeCodeCamp/league-for-good/issues/73)


### Day 6: January 4, 2018
1/4/2018, 8:51:21 PM

**Today's Progress**:

I continued with the fcc's sumPrimes challenge. I am currently experiencing a problem with input of 3.
I suspect I have a logic error with the for loop.

Also learned there's been a bit of lag with the console for Firefox and Chrome was not playing nicely either.
Perhaps because I decided to do a movie recording of my mug and screen recoding of my work during the 60 minutes.

**Thoughts**:

I refuse to give up on this challenge!

I feel like I'm really close to completing without having to look at the hints.

Recording with Quicktime (although may have affected computer's performance) while I worked and using Pomotodo kept me very focused and on task this evening.

**Link(s)**
1. [Pomotodo](https://pomotodo.com/)


### Day 7: January 5, 2018
**Today's Progress**:
Finished the fcc sumPrime challenge.
Started to initially figure out the next challenge, Smallest Common Multiples, by Googling the needed formulas.

**Thoughts**:

Glad the sumPrime challenge is finished. Ironically as I was nearing the end I found some tighter code within MDN docs:

```
function isPrime(element, index, array) {
  var start = 2;
  while (start <= Math.sqrt(element)) {
    if (element % start++ < 1) {
      return false;
    }
  }
  return element > 1;
}

console.log([4, 6, 8, 12].find(isPrime)); // undefined, not found
console.log([4, 5, 8, 12].find(isPrime)); // 5
```

I also found a bug in the fcc challenge as well. One of the test asks for the sum of of a prime:
```
sumPrimes(977) should return 73156.
```
I did ask this in the forum but I may have to raise the bug on Github.

The next challenge was a tad confusing. I did end up on the hint page and just read the top that indicated that the challenge required a range if given two numbers.

ie (1,5) = 1,2,3,4,5

Again, this should be a little more clear on the challenge than subtly mentioning it.

I have to use these formulas with all the numbers:

//gcd(a, b) = gcd(a - b, b)
//lcm(a, b) = a × b / gcd(a, b)


Found a few examples of this, apparently called "Euclidean algorithm".


```
function euclideanAlgorithm(a, b) {
    if(b === 0) {
        return a;
    }
    const remainder = a % b;
    return euclideanAlgorithm(b, remainder)
}

function gcdMultipleNumbers(...args) { //ES6 used here, change as appropriate
  const gcd = args.reduce((memo, next) => {
      return euclideanAlgorithm(memo, next)}
  );

  return gcd;
}

gcdMultipleNumbers(48,16,24,96) //8


```


**Link(s)**
1. [MDN find example](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/find)
2. [LCM](https://www.math.nmsu.edu/~pmorandi/CourseMaterials/LCM)
3. [GCD](https://www.math.nmsu.edu/~pmorandi/CourseMaterials/GCD.html)
4. [Euclidean algorithm](https://en.wikipedia.org/wiki/Euclidean_algorithm)


### Day 8: January 6, 2018
**Today's Progress**:
Started work on fcc's next challenge, smallestCommon. Finding solutions on Stackoverflow.com, very simple. Actually walking through the code and figuring out the what is happen... not so much.

Working progress but now grasp an example I was walking through and a repeat lesson on ES6 ...args and => arrow functions. I suspect I will have to hammer some of these gems down through late examples and projects.

**Thoughts**:
When reading someone else's code I tend to skip over what I assume is error check without questioning, because that's based on my style. Not realizing that's the key part I'm trying to figure out.

Trying to create the habit of going line by line.

**Link(s)**
1.[Great example by gwpmad](https://stackoverflow.com/questions/1231733/euclidean-greatest-common-divisor-for-more-than-two-numbers)


### Day 9: January 7, 2018
**Today's Progress**:
Continued working on FCC's challenge smallestCommon.

**Thoughts**:
My working progress is trying to glue 3 functions together. I know I'm probably not going the easiest route, but I will have to double check that I'm referencing the correct formula.

Probably run a few tests at lunchtime tomorrow. There's been a death in the family so this week will be tricky, but I will do my best to put my time in.

Was working with in the same room as the wife with TV in the background, that counts right... as quality time... with the wife? Regardless I was a little more cavalier and unfocused than usual.


### Day 10: January 8, 2018
**Today's Progress**:
Continued FCC smallestCommon challenge. Struggled for an hour than decided to look at the spoiler.

**Thoughts**:
Again, I was very close to the solution but not elegant as the provided spoiler. This goes back to my days of math homework and accounting. I learn better when the solution is available at the back of the book or some software provided. I'm wired for immediate feedback. I don't mind f'n around on my first attempt, but if I can look at more beautiful code I'll always do that after struggling long enough.


**Link(s)**
1.[smallestCommon spoiler](https://forum.freecodecamp.org/t/freecodecamp-algorithm-challenge-guide-smallest-common-multiple/16075)


### Day 11: January 9, 2018
**Today's Progress**:
Finished two fcc challenges :) ~ findElements; dropElements

**Thoughts**:
Both challenges were surprising easier than a few of the previous challenges. Earlier today was a family funeral so I'm actually surprised I was able to crank out 2 solutions after a very emotionally draining day.

Lesson learned today, show up and do the time... will probably surprise yourself of the results.


### Day 12: January 10, 2018
**Today's Progress**:
Worked on FCC's steamrollArray challenge. Nested arrays are more difficult than I thought. Carrying on with the theme of the last few challenges I am attempting to call another function that uses reduce on the array if isArray built-in function is true. Trying to do this with a for loop does not seem to be working. Perhaps using a While loop.

```
function steamrollArray(arr) {
// I'm a steamroller, baby
  for (i = 0; i < arr.length; i++){  // ==> For loop not working for me <==
    if (Array.isArray(arr[i]) ){
      flattened(arr);
    }
  }
  console.log("arr: " + arr);
  return arr;
}

function flattened(arr){
  return arr.reduce(
      ( acc, cur ) => acc.concat(cur),
      []
    );
}
console.clear();
steamrollArray([1, [2], [3, [[4]]]]);

```


**Thoughts**:
Challenge is fun but makes for some late nights. Ideally I would like to finish off FCC full curriculum within the R1; but if I don't move on to something else I'm can see myself getting bored. Perhaps that's the whole point of the challenge...pushing through that impulse.


**Link(s)**
1. [Code examples](http://www.jstips.co/en/javascript/flattening-multidimensional-arrays-in-javascript/)



### Day 13: January 11, 2018
**Today's Progress**:
Found a solution quickly on Stackoverflow, but trying to decode the why solution took up some time.


```
[0, 1, 2, 3, 4].reduce(
  function (
    accumulator,
    currentValue,
    currentIndex,
    array
  ) {
    return accumulator + currentValue;
  }
);


// test ? expression1 : expression2  

var now = new Date();  
var greeting = "Good" + ((now.getHours() > 17) ? " evening." : " day.");  

```
**Thoughts**:

I certainly need more practice with callbacks and tracing.

**Link(s)**:

1. [Flatten Function](https://stackoverflow.com/questions/10865025/merge-flatten-an-array-of-arrays-in-javascript)



### Day 14: January 12, 2018
**Today's Progress**:

Completed another fcc challenge, binaryAgent.

Found another snippet on Stackoverflow. It had some addition false parms, which I could not reference any value so I was able to take it out.

Binary code => parseInt(string,2) => String.fromCharCode //ASCII translation

The parseInt() function parses a string argument and returns an integer of the specified radix (the base in mathematical numeral systems).

```
function binaryAgent(str) {
  var splitArr = str.split(' ');
  var strResult = "";
  for (i = 0; i < splitArr.length; i++){
    var strDecoded = String.fromCharCode(parseInt(splitArr[i],2) );
    strResult = strResult.concat(strDecoded);
  }
  return strResult;
}

console.clear();
binaryAgent("01000001 01110010 01100101 01101110 00100111 01110100 00100000 01100010 01101111 01101110 01100110 01101001 01110010 01100101 01110011 00100000 01100110 01110101 01101110 00100001 00111111");

```

**Thoughts**:

Working from Mom's, just before dinner. We had another funeral today (second one of the week :(( ).
Able to stick with the challenge and working in between the chaos of life.
Focus was again oddly sharp despite thinking I would not deliver. Just showing up and working on the problem with no expectation seems key to better results and output.

1/13/2018, 12:53:46 AM

Some late night coding at Ma's while watching Dirk Gentley. Almost have the next fcc challenge completed. Once again I'm stumbling to figure out Object Collection.



**Link(s)**
1. [stackoverflow snippet](https://stackoverflow.com/questions/21354235/converting-binary-to-text-using-javascript)

The parseInt() function parses a string argument and returns an integer of the specified radix (the base in mathematical numeral systems).


### Day 15: January 13, 2018
**Today's Progress**:

Continued work on fcc challenge, truthCheck.

In the middle of time while looking up something on Stackoverflow I ran into the developer annual survey and decided to take the time to do it.

I thought I crack the fcc challenge. So very close but still missing how to iterate through a collection of objects.



```
if( value ) {
}
```
will evaluate to true if value is not:

null
undefined
NaN
empty string ("")
0
false


1/13/2018, 10:09:09 PM

Last attempt and drive worked! :)

```
function truthCheck(collection, pre) {
  // Is everyone being true?
  for (var k in collection) {
    console.log(  collection[k][pre]);
    var preValue = collection[k][pre];
    if ( !(pre in collection[k]) || (!preValue)   ){
      return false;
    }
  }
  return true;
}
console.clear();
truthCheck([{"user": "Tinky-Winky", "sex": "male"}, {"user": "Dipsy", "sex": "male"}, {"user": "Laa-Laa", "sex": "female"}, {"user": "Po", "sex": "female"}], "sex");
```

**Thoughts**:

Collection of object are frustrating, but found a solution on Stackoverflow.
Instead of a for loop I was able to step through with:  for (var k in collection)

**Link(s)**
1. [Iterating for a collection](https://stackoverflow.com/questions/15282480/iterate-over-a-collection-of-objects-in-javascript-and-return-true-from-that-fun)


### Day 16: January 14, 2018
**Today's Progress**:

Watch a YouYube video by Scott Hanselman, Scaling Yourself. Although not coding, it was totally worth it and a meta way to look at the week coming up.

For the fcc challenge I worked on the addTogether function for about 45 minutes and then looked at the spoiler. Once again pretty close. I always prefer looking at the Advanced solution.


```
//jshint esversion: 6
function addTogether() {
  var args = Array.from(arguments);
  return args.some(n => typeof n !== 'number') ?
    undefined:
    args.length > 1 ?
      args.reduce((acc, n) => acc += n, 0):
      (n) => typeof n === "number" ?
        n + args[0]:
        undefined;
}
```

Going to spend what little time I have left hanging with the wifey. :)

**Thoughts**:
**Link(s)**
1. [Scott Hanselman, Scaling Yourself](http://youtu.be/IWPgUn8tL8s?a)


### Day 17: January 15, 2018
1/15/2018, 10:06:28 PM

**Today's Progress**:
Walked through the advanced spoiler solution for addTogether. The nested ternary operator gave me pause.

Started working on the next solution for fcc challenge telephoneCheck. Already found a template on Stackoverflow.

**Thoughts**:

Looking through the spoilers and checking Stackoverflow seems like cheating and cutting corners.

However I'm reminded of a lesson I learned exactly 8 years ago. I was an avid skydiver and decided to take  a Parachute Rigging Course down at ParaLoft with Handsome David DeWolf in Elizabethtown, Pennsylvania.

Some of the rough tough guys suggested we try closing our 25 supervised reserve rigs with might and muscle alone. A friend of mine that I made on the course that worked at Sunrise in Florida, manufacturer of Wings parachute containers. Although experienced to some degree he finished the required course load in a 1/3rd less time than everyone else. When I asked him how he was so fast, he showed me. Rather than might and muscle he reached over and grabbed the same tools that were sitting next to me and readily available and showed me how to close a parachute container with no effort at all. It seemed so easy that it actually felt like cheating. It took many years to full absorb what he taught me. Check the ego at the door and measure the results.

Finding and utilizing the easy way will reduce the wear and tear on me.

**Link(s)**
1. [Ternary operator more than one condition](https://www.codecademy.com/en/forum_questions/50a735d192bf860b2000077c)
2. [Stackoverflow examples](https://stackoverflow.com/questions/4338267/validate-phone-number-with-javascript)


### Day 18: January 16, 2018
**Today's Progress**:
Completed fcc challenge telephoneCheck.

**Thoughts**:

Found a great regex tester tool that gave me a way to list all of my test data and then play around until everything was passing. I think there may be an error with one of the tests. I submitted it to the forum for review.

Long night after Toastmaster (7pm - 9'ishpm). Will have to schedule my coding hour during lunch on Tuesday from this point on.

**Link(s)**
1. [NANP explained](http://en.wikipedia.org/wiki/North_American_Numbering_Plan)
2. [stackoverflow example 1](https://stackoverflow.com/questions/4338267/validate-phone-number-with-javascript)
3. [stackoverflow example 2](https://stackoverflow.com/questions/45620551/understanding-regexp-for-area-code-phone)
4. [regex tester](https://www.regextester.com/17)


### Day 19: January 17, 2018
**Today's Progress**:

1/17/2018, 3:44:16 PM

Started to do a few exercise and review some of the suggestions of the next fcc challenge, updateRecords.

JSON seems pretty straight forward.

Also looked at the actual issues for freecodecamp on Github, and started to look at how to contribute.
This has led to a tiny rabbit hole updating my Mac's homebrew and Node.js - still going.

**Thoughts**:

The 100DaysOfCode challenge is putting some tension with my S.O. Usually I spend my hour on the couch while my wife and I watch some Netflix. She's mentioned she's not thrilled with my spending time on focus coding, rather than her.

Thus I experimented with doing my hour while junior was napping (sick day today). He's up and about and running around as I type.

This is truly a challenge of time management. How does divide up work, family, fitness, a 100Day challenge, and finally sleep within 24 hours?

Ideal
-----
8 - work
8 - sleep
1 - 100DaysOfCode
1 - fitness
6(?) - family/misc  

**Link(s)**
1. [contribution-guidelines](https://github.com/freeCodeCamp/freeCodeCamp/blob/staging/CONTRIBUTING.md#contribution-guidelines)


### Day 20: January 18, 2018
**Today's Progress**:
Started to get traction on the updateRecords freeCodeCamp challenge.

**Thoughts**:
Was VERY squirrelly tonight. I had a personal coaching session, and then creeped and VERY successful person from high school. Probably one of the top successful people ever to attend my highs school.

Was not a very focused session, but very enlightening.


### Day 21: January 19, 2018
**Today's Progress**:

Continued work on updateRecords challenge.

**Thoughts**:

Not sure why I'm unable to make dot notation work, but the [] notation worked fine.

Err... found the answer right in the instruction (ref: link 1 below).

Very close to completing challenge but I went on a bit of a tangent with trying to match existing values. I'm thinking this is not necessary for this exercise as they've set up particular test to pass.

However this lead me to the 2 interesting links below on equations for partial string matching we've become so accustomed for input forms.


**Link(s)**
1. [Explanation on bracket notation](https://www.freecodecamp.org/challenges/accessing-objects-properties-with-variables)
2. [Compare String Match Likelihood](https://stackoverflow.com/questions/10473745/compare-strings-javascript-return-of-likely)
3. [Levenshtein_distance](https://en.wikipedia.org/wiki/Levenshtein_distance)


### Day 22: January 20, 2018
**Today's Progress**:

1/20/2018, 10:20:31 PM

Finished updateRecords, while drinking brews and watching Netflix with bro-inlaw.

**Thoughts**:

Did not want to do challenge today. A tad hungover from BD party last night. But finished the challenge one test at a time.

**Link(s)**
1. [push value to array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push)
2. [adding element to JSON object](https://stackoverflow.com/questions/28527712/how-to-add-key-value-pair-in-the-json-object-already-declared)


### Day 23: January 21, 2018
**Today's Progress**:
Started work on Symmetric Difference FCC challenge.

**Thoughts**:
This appears to be another area of Algebra I'm not familiar with. There's some massive gaps I have... ie. never took calculus before and never stopped to learn that despite half ass efforts. Now there's areas of algebra that I don't know about either.

May have to grab a book or take a class for some refresher math.


**Link(s)**
1. [Diff between algebra and calculus](http://www.differencebetween.net/science/difference-between-algebra-and-calculus/)
2. [Symmetric Difference](https://www.youtube.com/watch?v=PxffSUQRkG4)


### Day 24: January 22, 2018
**Today's Progress**:
Worked tonight with a buddy on a startup idea, including SWOT, and setting up a repo.

**Thoughts**:
This venture is exciting already giving me an idea of the work and progress working remotely in development.


### Day 25: January 23, 2018
**Today's Progress**:
Worked again on fcc challenge sym. Issue mastering .reduce function.

**Thoughts**:
This should be a relatively easy challenge in concept but I'm not see the simple solution.
I think there's something to the effect of going through all the arrays and removing all the numbers with one or more matches.

Long day was not really in the mood to code, but put my time in regardless.


### Day 26: January 24, 2018

1/24/2018, 11:45:46 PM
**Today's Progress**:
Work continues with sym fcc challenge. I feel I'm very close but stuck on the ternary condition.

**Thoughts**:
The challenge is keeping me engaged enough not to cheat this time. I'm see some progress in the console.log, however stumped why the ternary condition refuses to work.

So confused that I actually posted a question on Stackoverflow. It's very rare that I actually post a question. But my unique example and married to my code made me keen on posting like a noob.

The idea of asking for help online is something I have to perfect. I shy away from looking like a dumbass, but time to get over myself.

The challenge is also wearing on my marriage.:S
Wife is so not thrilled I'm only 1/4 of the challenge done and not going to bed at an ideal time of night.
A random phone call put me behind schedule from my usual 9pm-10pm coding session.

My path and purpose is to get to mastery.



1/25/2018, 12:03:56 AM

Received an answer already on Stackoverflow, and now I have a few more passing tests on sym. :)




**Link(s)**
1. [Stackoverflow question](https://stackoverflow.com/questions/48435789/slicing-doesnt-work-in-ternary-conditional)


### Day 27: January 27, 2018
**Today's Progress**:

Finished setting up freeCodeCamp on localhost.

**Thoughts**:

Missed yesterday because I needed sleep more.
Tonight is the same.
Less code but rather more setup.
Will log a decent hour tomorrow.


==============================================
### Day 01: February 8, 2018
**Today's Progress**:
Starting over.

Day 1 of 4 for Freekend Hackathon 2018~ ParaPOS

**Thoughts**:
I made it > 25% last #100100DaysOfCode challenge, then was derailed by a house project to redo my office (took approximately a week).

I'm starting the challenge again with a free weekend (Freekend) Hackathon.

After my family returns I require a more sustainable routine other than late night coding. It was putting a strain on my marriage.

I am thinking a possible solution is to become an "SUPER" early riser. Wake up before or at 5am and get an hour of coding in OR at the very least 30 minutes of coding, then knock of the rest off at lunch time or in the evening.


**Link(s)**
1. [Freekend Hackathon](https://github.com/paulywill/freekend-hackathon-2018)


### Day 02: February 9, 2018
**Today's Progress**:

Day 2 of Freekend Hackathon.
Still going though the Getting Started Guide (again).

**Thoughts**:

Slow and steady.
Moneyball playing is both nice company alone and a distraction.

**Link(s)**
1. [Day 2 vlog](https://youtu.be/K0EigxhpIug)
-------------------------------
### Day xx: Month Day, 2018
**Today's Progress**:
**Thoughts**:
**Link(s)**
1. []()
-------------------------------
