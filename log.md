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


### Day 03: February 10-11, 2018
**Today's Progress**:

Pagination. Finished Getting Started Guide (mostly).

**Thoughts**:

Solid template to show user tomorrow (later this morning).

**Link(s)**
1. [YouTube Day 3](https://youtu.be/D6bBiFISQvw)


### Day 04: February 11-12, 2018
**Today's Progress**:

User feedback; started the Rigs portion of the packing POS project.

End of my Freekend Hackathon.

**Thoughts**:
I'm going to regret not going to bed earlier.

2/12/2018, 2:26:20 AM

**Link(s)**
1. [Day 4 of 4](https://youtu.be/wm9Nc5-V4_g)


### Day 05: February 13, 2018
**Today's Progress**:

Continued work on the Parapos from the Freekend Hackathon. Decide to make its own repo on Github.

Currently trying to figure out how checkboxes work in Rails 5. Rigs status is not reflecting in the database.


**Thoughts**:

Rails is a pain the ass sometimes. Pissed off that when I search for information that I'm directed to a book that is priced well above $100 to access all the bells and whistles.

I also setup a slick IRC in the iterm2, irssi to log into the Freenode #rubyonrails channel only to find little or no activity in the channel.

Thinking perhaps it was something wrong with the client I logged into the #python channel and the activity is crazy.

I'm determined to master RoR, but I am paying attention to how the communities are behaving. There seems more passionate people in the Python community. I know this is not a fair comparison as I should be saying "Ruby on Rails" vs "Django" and not just python the language.


**Link(s)**
1. [Parapos Github](https://github.com/paulywill/parapos)


### Day 06-07: February 14-15, 2018
**Today's Progress**:

Still working on ParaPOS.

Did a bit of research and reading on V-Day during the day on using Chef and hosting a RoR on Linode.

Think I found some leads when I'm at that stage.


Tonight (Feb.15) worked on the Rigs link on the Packjob index screen. I thought something was getting truncated... not the case.

Now trying to resolve drop-down boxes again.


**Thoughts**:

Very tired.


**Link(s)**
1. [Chef and Linode](http://www.talkingquickly.co.uk/2013/09/using-chef-to-provision-a-rails-and-postgres-server/)


### Day 08-09: Month Day, 2018
**Today's Progress**:

Yesterday I resolved the dropdown, but regressed on the index showing the rigs properly.

Today I added a reference (a db join) between packjobs and rigs. Although was was getting the links to work before... I think there's some redundancy going on.


**Thoughts**:
Sometimes frustrating running into errors and mad searches on Stackoverflow. However I'm starting to understand the error messages more how to troubleshoot a little better.


**Link(s)**
1. [sqlitebrowser](https://github.com/sqlitebrowser/sqlitebrowser)
-------------------------------
### Day 01-04: September 12, 2018
**Today's Progress**:

Finished all the new lessons of the first certification for FCC's "Responsive Web Design Certification".

I never did take the time to do nitty gritty studying of CSS front-end, so I was thoroughly impressed with the lessons. I still have to do the few projects and the FCC's TDD CDN (quick a few acronyms there) make the process much more fun and interactive.


As well, I've jumped back into helping with some issues for the "[League for Good](https://github.com/freeCodeCamp/league-for-good)" project. In particular cleaning up some es-lint errors that my Atom IDE was picking up (easy to fix, but tedious help).


**Thoughts**:

I have a AWS test on the 28th this month. Part of my coding is getting into the mind set, but also a "slight" procrastination from some of the studying. Coding is much more enjoyable.

Using [Pomotodo](http://pomotodo.com) is helpful for knocking out my coding time. Working from home also helps with sticking to this challenge. More than anything, since this another attempt at 100DaysOfCode, the major lesson I learned is not "always" doing my coding during what should be "quality time" with my wonderful and patient wife.

I can do it at lunchtime or between my Pomotodo breaks from work.

In addition since I've been applying for more jobs, I've learned from some very polite rejections that I have to go from *Good* to _**GREAT**_. 100DaysOfCode can help me get there.  

**Link(s)**
1. [freeCodeCamp's Testing Suite](https://github.com/freeCodeCamp/testable-projects-fcc)



### Day 05-06: September 14, 2018
**Today's Progress**:

Yesterday was doing more AWS studying, covering DynamoDB. Yikes, much to review!!!

Today tackled some more FCC project, "[Survey Form](https://codepen.io/paulywill/pen/PdepxV)". Very much work in progress, but all the TDD tests are passing.


**Thoughts**:

Just listened to the podcast on [100DaysOfCode](https://www.freecodecamp.org/news/quincylarson/100-days-of-code-creator-alexander-kallaway--bkuL0lP20). Very impressed! Did read several of the books mentioned, but would love to re-read them again. Some are new mentions I've never heard of and actually just reached out to Alexander if there was a list, as I wasn't able to find good show notes.

Have to get ready for a wedding now.




### Day 07: September 15, 2018
**Today's Progress**:

More AWS studying. Officially finished cloudguru's Udemy AWS Developer Associate 2018 course.

**Thoughts**:

Still so many gaps and nitty gritty to cover.
Would like to do some more studying and coding tonight when junior is put to bed.



### Day 08: September 16, 2018
**Today's Progress**:

Even more AWS studying. Finished another AWS test, 64%.

**Thoughts**:

I'm fucked if I don't study even more!

**Link(s)**
1. [AWS Practice Tests](https://www.udemy.com/aws-certified-developer-associate-real-tests-o)



### Day 09: September 17, 2018
**Today's Progress**:

AWS studying, ElastiCache.

Upon reviewing my practice test yesterday one of the questions I flunked or totally gapped was ElastiCache.

So tonight I dedicated the entire night learning and doing some AWS Getting Started lab on ElastiCache Redis cluster.


**Thoughts**:

As always the mild coding and actual labs and working with AWS is much better than just reading.

I know in my heart doing this AWS studying under the #100daysofcode challenge is forcing me to put my much needed studying time in.

Whao... and where the hell have I been to not know about TCL/TK?

```
Tcl runs the operator interface of a Shell Oil drilling rig, runs the NBC network control system 24x7, has been used to program the Hubble Space Telescope and prototype the Mars Pathfinder, is hiding in every Tivo box and many Oracle products. Don't forget companies like Pixar, Motorola, IBM, Sybase, Nortel, Raytheon...
```

I had to 'sudo yum install tcl' to run the 'make test' for the source for redis on the EC2 instance.

Reading about what TCL/TK has been used for is bonkers!

AND... watching the tests pass for 'make test' is somehow old school linux startup sexy for me. :S

\o/
 |
 ^

**Link(s)**
1. [AWS Redis ElastiCache Getting Started](https://docs.aws.amazon.com/AmazonElastiCache/latest/red-ug/GettingStarted.html)
2. [TCL/TK Audience](https://www.tcl.tk/about/audience.html)




### Day 10: September 18, 2018
**Today's Progress**:

Pretty zonked from fixing mainframe issue all day for work.

Did some code review for League-for-Good, after learning about fetching someone else's remote branch.


**Thoughts**:

Sometimes in an effort to get things working we gloss over the details. It is only when something refuses to work do we address the details.  -me




### Day 11-12: September 19-20, 2018
**Today's Progress**:

More and more AWS studying.

Found a great list of questions to review, even gave props to the author yesterday on Twitter.

In addition, yesterday, I connected with the local coders and going to check out a weekend hackathon for browser extensions creation for Chrome at my old college. :)

I did throw my hat in the ring as well for a volunteer job with www.canadalearningcode.ca, for the Barrie chapter.

There's a thriving community in my very own city I'm not even taking advantage of.


**Thoughts**:

A HUGE knowledge gap is all the APIs and error messages. A habit from my work is not committing much to memory and creating a library of documentation to looks up everything.

Seems there's no way around this, I need to commit to memory some of the functions and errors or at least see if there's a pattern.

I am starting to feel the fire under my ass, I have officially reached the 7 days until my scheduled exam.


**Link(s)**
1. [Study List - 55 THINGS YOU SHOULD KNOW FOR THE AWS CERTIFIED DEVELOPER ASSOCIATE EXAM](https://www.cozero.com.au/news/2018/55-tips-for-aws-developer-associate-exam.html)
2. [canada learning code](www.canadalearningcode.ca)



### Day 13-14: September 21-22, 2018
**Yesterday's Progress**:

Started to finally read up the FAQ for DynamoDB and started to learn Global Secondary Indexes more. Still have to dive into what Local Indexes are and some other nitty gritty.


**Today's Progress**:

Full nerdery day! :)

Went to the browser extension workshop today. Some advance people and some beginners. Not baad overall... I did learn a few things.

**Thoughts**:

I was getting annoyed at the workshop when people I didn't know, the "mentors", were sort of lurking over my shoulder watching me code. I was so not use to that and something I'd probably have to get over if I were to pari program. I actually have no issue in someone is sitting next to me we're working together... but "shoulder readers" set off my spidey sense big time.

It would be neat to have a program that takes a picture of anyone reading your screen over your shoulder and do facial recognition and social media search in real-time in-front of them. :P


### Day 15: September 23, 2018
**Today's Progress**:

AWS studying continues... and probably will be all week.
Started to create a view online flash cards on Quizlet; more FAQ reading on DynamoDB; and another practice exam with a higher mark.

**Thoughts**:

Absolutely zonked today. Was up late last night (3am'ish) doing some parachute rigging for a friend. Naturally our toddler decided not to sleep and the wife... we were all grumpy today and made studying a tad challenging.

Onward!

**Link(s)**
1. [Quizlet - Flash cards](https://quizlet.com/)
2. [Udemy AWS CDA Practice Tests](https://www.udemy.com/aws-certified-developer-associate-real-tests-o/)


### Day 16: September 24, 2018
**Today's Progress**:

More AWS studying. Everything is slow at work because a tornado hit Ottawa over the weekend. :/

**Thoughts**:

I'm slowly cramming more cloud computing concepts into my grey matter. Nitty gritty (ie API names and error codes) will be a last minute binge.



### Day 17: September 25, 2018
**Today's Progress**:

Guess what? Yup, more AWS studying.

**Thoughts**:

Making some slow but consistent progress reviewing practice tests and the related FAQS and other miscellaneous.


### Day 18-20: September 28, 2018
**Today's Progress**:

Passed the AWS Developer Associate test!

**Thoughts**:
Taking the weekend off to recover.

**Link(s)**
1. [AWS Certified Developer - Associate - License 5ZW44XL2KJVEQ7CJ](https://aw.certmetrics.com/amazon/public/verification.aspx)



### Day 21: October 1, 2018
**Today's Progress**:

Started the TDD, "Obey the Goat", book again in preparation for PyCon Canada 2018 in November.

**Thoughts**:

My evil plan B to pivot in my career is nicely underway.

AWS certification -> check.
Python mastery -> in progress.


**Link(s)**
1. [Test-Driven Development with Python: Obey the Testing Goat: Using Django, Selenium, and JavaScript](https://amzn.to/2OYjR0F)
2. [PyCon Canada](https://2018.pycon.ca/)



### Day 22: October 2, 2018
**Today's Progress**:

Once again tackling TDD book, on chapter 4.
Love [this cartoon](http://hyperboleandahalf.blogspot.com/2010/06/this-is-why-ill-never-be-adult.html) they cite.

**Thoughts**:

Day job is becoming a toxic battle rather than a Meritocracy and one of required technical aptitude.

Life is becoming shorter for such a place.



### Day 23: October 3, 2018
**Today's Progress**:

Sick day. More TDD book. Meh.



### Day 24: October 4, 2018
**Today's Progress**:

TDD book, finished chapter 4.

**Thoughts**:

This with be what I will be doing for the rest of the month... hell or high water.



### Day 25: October 5, 2018
**Today's Progress**:

Chapter 5 of the TDD book. Looked into and added other books mentioned on my to-do list.

**Thoughts**:

More demotivating fighting with management at the day job as a Systems Programmer for Mainframes for the Government of Canada.

On the other end of the spectrum I'm more than happy to volunteer my free time to helping FCC, and Quincy Larson, with open source initiatives.


### Day 26-28: October 6-8, 2018
**Today's Progress**:

Saturday, spent some time watching a video that's been sitting in my inbox for some time now, on [Dev Tools in Chrome](https://www.youtube.com/watch?v=wz1Sy5C039M).

Sunday, spent the afternoon getting pylint and VScode setup nicely. I think I'm now smitten with VScode compare to Atom.

Thanksgiving Monday, had an amazing video call with the man himself behind FCC, Quincy Larson. Walked me through the QA workflow for the FCC guide repo for incoming PR they needed help with. I spend a few hours tonight trying my best to make a dent. 


**Thoughts**:

Was very impressed with how easy it was to talk to Quincy and learn via Google Hangout. Cannot wait to contribute and help even more in the project.


### Day 29-31: October 9-11, 2018
**Today's Progress**:

For the past two days been focusing on FCC QA'ing with PRs for the [guide](https://github.com/freeCodeCamp/guide). Quincy Larson is going to archive it in the VERY near future for a future Intenational version. Very exciting.

Going to continue with my TDD Obey Goat between my [pomotodos](https://pomotodo.com/app/).


**Thoughts**:

Was on-site at work. Meh. Don't know if I'm any longer built for office life compared to WFH. The majority of the day is burnt trying to setup a proper workstation and workflow.


### Day 32-33: October 12-13, 2018
**Today's Progress**:

Yesterday I spent some time prettier up my FCC survey project. Although the objective is rather easy it took some time to dissect the CSS from the example and make it work for my own.

Then I'm thinking of adding some extra CSS generated graphics in the background and borders.

Tonight I spent about an hour closing some more QA for FCC's guide. 

**Thoughts**:

I really want to focus more on coding for the rest of the month. I count all nerdery (ie learning, doing OSS work, setting up my IDE) as part of the challenge... but I'd really like to make more things and code more.

**Link(s)**
1. [Survey Project](https://codepen.io/paulywill/pen/PdepxV?editors=1000)
2. [Biohazard Graphic Example](https://codepen.io/gutsgaurav/details/GqaGQV#forks)
3. [FCC's New Guide PRs](https://github.com/freeCodeCamp/freeCodeCamp/pulls)


### Day 34: October 14, 2018
**Today's Progress**:

TDD Goat book continues.
Decided to submit Survey project with fancy animation for now.


### Day 35: October 15, 2018
**Today's Progress**:

More TDD book. Did not get around to FCC PRs b/c of day job. Maybe tomorrow.

**Thoughts**:

The TDD book is little a little frustrating as it tends to quickly go off the rails for me. As life normally does. ie I forced the migrate command earlier than indicated in the book b/c I believe I was missing a def method_name.

The result? I get to the same place, but went a different route than the author intended. I suppose I learn more from my "Choose Your Own Adventure" path.


### Day 36: October 16, 2018
**Today's Progress**:

TDD chapter 5 continues at the Barrie Public Library.

**Thoughts**:

Tired. Little scattered today with productivity and focus.


### Day 37-38: October 17-18, 2018
**Today's Progress**:

Yesterday, as they legalized marijuana our Internet in Ontario crashed for several hours. No cause and effect I'm sure.

As result I did a very tiny bit of TDD goat book offline. This was just before the family and I went to The Wiggles Show. :P 

Today I put the wheels in motion for a tiny React project among some others that are interested in doing some online remote programming. So far... React is installed on Heroku.


**Thoughts**:
People are really keen to help with OSS. Love it!


**Link(s)**
1. [React Project - Seinfeld Strat App](https://github.com/paulywill/seinfeld-strat-app)
2. [Heroku: Seinfeld-Strat-App](https://seinfeld-strat-app.herokuapp.com/)


### Day 39-40: October 19-22, 2018
**Progress**:

Saturday will not count towards the challenge as the day was devoted to yardwork and driving my wife to her first bar gig with her band. :)

Sunday I was feeling very green but managed to complete a few PRs for myself for the Hacktoberfest, in particular when I was going through SASS curriculum and notice some gaps in explainations and solutions.

Whether I receive a t-shirt at this point would be gravy.

Tonight, I secured the final PR for the free t-shirt, and completed the SASS section. I feel I slipped on my intention to finish the TDD Goat book with this additional Seinfeld-Strat-App, but .. meh. I'm having fun and learning regardless.

I DID totally f*ck up tonight though. While trying to quickly resolve and clean up my S3 files I accidentally, without reading carefully, a provision unit which apparrently billed me $100 USD! For retrieving in a region I have little or no data. Ahhhh AWS, I bow to you once again.


**Thoughts**:

AWS is costing me so much for my carelessness.

**Link(s)**
1. [Hacktoberfest Stats](https://hacktoberfest.digitalocean.com/stats/paulywill)
2. [AWS Expensive Lesson - Provisioned expedited retrieval](https://aws.amazon.com/glacier/pricing/)


### Day 41-43: October 23-26, 2018
**Progress**:

Starting to slip on the challenge.

Lots of solid hours this week working on PRs for FCC and learning about testing suites. I'm digging the concept behind cypress.io

Tonight I'm zonked and not counting but I think I have a start-up idea in the works.

Day job is giving me grey hairs and grief.


**Thoughts**:

Sleep. Early 5:30am wake up experiment is taking toll.



### Day 44: October 27, 2018
**Today's Progress**:

FCC curriculm React, in the front-end certificate portion.

I'm poking about in the new curriculm at FCC and circling back to the previoius certicates I'm almost done.

The "Product Landing Page" looks like a handy project to complete. My portfolio page also needs some fixing up.


**Thoughts**:

I went down a few rabbit holes tonight, like I normally do. I'm on a recent kick looking at front-end illustrators using either Illustrator or some kick ass CSS.

As well my tradition to prove a theory is still holding true to some extent. Whenever I'm on a page and click on "Careers" and almost always have a jobs posting. Now more than ever I'm also seeing "Remote Friendly", which excited me to no end. It also unfocuses me because the tech stack often changes from posting to posting.

Do I really want another job or to become a founder?

**Link(s)**
1. [Impressive CSS Illustration](https://codepen.io/agathaco/pen/bRxYxL)
2. [Illustrator](https://dribbble.com/shots/5458845-Awkward-Coincidence)


### Day 45-48: October 28-31, 2018
**Progress**:

Nothing but lots of FCC QA'ing and helping. Still trying to wrap my mind around the testing suites and setup for the FCC / Travis CI builds.

There was an issue I was trying to help and investigate with and it was gond show trying to figure out all the products and pieces.

**Thoughts**:

Mountains to climb still. Thankfully some of the pieces are actually part of the curriculm. In the meantime I want to dedicate my space cycles to learning Unit Testing and Integration Testing.

**Link(s)**
1. [FCC testing issue](https://github.com/freeCodeCamp/freeCodeCamp/issues/30709)
2. [AVA JS - unit testing](https://github.com/avajs/ava)
3. [Mocha - browser testing](https://mochajs.org/)


### Day 49-50: November 2;5, 2018
**Progress**:

Thursday and Friday night I spent once again QA'ing PRs for FCC.

The weekend I was completely unplugged and wayyyy up north off the grid visiting some friends. It was a nice little vacation.

Today I struggled through the time change working from home on my usualy tech stuff, but did manage to just finish my hour on the React lessens on FCC.

The super strong IPA beer at dinner was a rather unproductive decision in hind sight.

**Thoughts**:

PyCon Canada 2018 this weekend. I'm going to be taxed Saturday me thinks with another engagement in the evening. The T.O. commute, while not impossible, is often a drag. May consider taking the train.


### Day 51-53: November 14, 2018
**Progress**:

Getting heat as I type this from the wife.

But, not withstanding I have been slacking on hitting the challenge mark every day in a row... but I refuse to start over as a family man. I'm going to put my time in but it might have some family time gaps.

Last weekend November 10-11, was PyCon Canada 2018 in Toronto. It was a nice level up and meeting some people and learning what's trending in the dev world relating to Python.

Tonight got back in TDD Goat book.

Tomorrow I will also be back on track.


### Day 54: November 15, 2018
**Today's Progress**:
Officially finished chapter 5 and 6 of the TDD book. Some of this is familiar. I have a long way to go before mastering TDD and Django!

**Thoughts**:
Was vvvvvery tempted to not clock in tonight. But on EDM and clocked in. Glad I did!

**Link(s)**
1. [EDM - Aural Therapy](https://househunters.podbean.com)


### Day 55: November 16, 2018
**Today's Progress**:

Started chapter 7 of TDD Goat Book... added another FT.

**Thoughts**:
Quite A.D.D. today with day job WFH.
Starting to cabin fever and need to work at coffee shop and/or co-working place; and or actual work building that's a pain in the ass to drive to.


### Day 56: November 17, 2018
**Today's Progress**:
More TDD Goat book, chapter 7... refactoring and more tests.

Single parent tonight... hope it's not an early morning :S

**Thoughts**:

1. My boss expressed token concern I do late night work *head shake*

2. Mr. Robot is a great but distracting show to watch while coding.

### Day 57-64: November 18, 2018
**Progress**:
Been tackling the TDD Goat book more slowly than anticipated.

Trying to absorb as much about Django and TDD in general.


**Thoughts**:
Finding the discpline and time to code is so difficult, but I am still putting my time in here and there. The bad habit of not updating this log is also getting out of control.

My obsession of looking at Remote DevOps job postings, and trying to grow a beard are also competing for my spare cycles and brain power.


### Day 65: November 26, 2018
**Today's Progress**:

Today was certainly a mild coding day. Spent spare cycles setting up two Fedora VMs. One server one desktop. I've decided (even though I love my OSX) need to keep my Linux skills sharp as per a suggestion from a Medium article.

**Thoughts**:

Was a little stir crazy today. Would be nice to work at co-working place tomorrow.

**Link(s)**
1. [How to become a DevOps...](https://medium.com/@devfire/how-to-become-a-devops-engineer-in-six-months-or-less-366097df7737)


### Day 66: November 27, 2018
**Today's Progress**:
- Helped identify security issue in FCC thanks to [tip on Twitter](https://twitter.com/sugarpirate_/status/1067147512065085442).

- Learned some interesting arguments for UNIX [find command and 2>/dev/null](https://medium.com/@codenameyau/step-by-step-breakdown-of-dev-null-a0f516f53158) that found secuirty issue


**Thoughts**:

Enjoying the ambience of my co-working home, [TCS in Barrie](https://thecreativespace.ca/), as much as possible before this location closes for good. :(

Will do some more TDD Goat book after day job work.

**Link(s)**
1. [FCC PR - #34469](https://github.com/freeCodeCamp/freeCodeCamp/pull/34469)
2. [hackerNews - event-stream](https://thehackernews.com/2018/11/nodejs-event-stream-module.html)


### Day 67: November 30, 2018
**Today's Progress**:
Finished chapter 7 and chapter 8 today.

Some solid coding at lunch time and this evening.

**Thoughts**:
This are starting to pick up again this time around with this book.

After finishing it, I'll have to dive deeper into making test from scratch for myself rather than copying code and logic. TDD is certainly not natural but still so pwerful I cannot deny its adoption.


### Day 68: December 3, 2018
**Today's Progress**:
Working through chapter 9 in the TDD Goat Book.

**Thoughts**:
I do remember doing this chapter last year and setting up on Linode, this time around trying to setup on AWS.. so far so good.

Curious that TOR is giving my immediate result and yet Chrome and Firefox is taking an extra long time for the DNS to be resolved since I set it up.

**Link(s)**
1. [Live Server](http://superlists.skillfol.io/)

### Day 69: December 4, 2018
**Today's Progress**:
More chapter 9 of TDD Goat book.
Long day.


### Day 70: December 5, 2018
**Today's Progress**:
Finished chapter 9 of TDD Goat book.

**Thoughts**:
Sick and feeling it.

**Link(s)**
1. [Staging Server](http://superlists-staging.skillfol.io/)


### Day 71-72: December 6-7 Day, 2018
**Progress ?**:

Spent quite a bit of time setting everything up on AWS EC2. Then chown recursively myself out of access (following a security article blindly). Was very close to fixing up the EC2 and retrieving new keys... but then accidentally deleted my EC2 volumes instead of DETACHING them.


**Thoughts**:

So easy to make major mistakes on AWS. I should have used SNAPSHOTS and/or learn about some other backups to the volumes for such an event.

It's a good cheap lesson and gives me even more practice going through the setup steps again.

**Link(s)**
1. [Security article I blame](https://plusbryan.com/my-first-5-minutes-on-a-server-or-essential-security-for-linux-servers)
2. [EC2 Key Pairs](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html)


### Day 73: December 8, 2018
**Today's Progress**:
Finally got back on track and at the end of chapter 10 of TDD Obey the Testing Goat again.

Some interesting gotchas along the way. Setting up Elastic IP with my EC2 instance so I can recycle away and not be affected.

There was a very subtle typo in my service that was preventing things start up clean and I kept getting 502 server error message.


**Thoughts**:
Despite holding a certification in AWS, working experience is something I have to be mindful of. 



### Day 74: December 10, 2018
**Today's Progress**:
Tackling chapter 11, automating all the steps from cahpter 9 and 10, in the TDD Obey the Testing Goat book.

Took my time disecting every line this time rather than copying code and running.

**Thoughts**:
Impressed with the Fabric deployment tool.

Did a rookie mistake, update a dependency on the production server without first checking on my local.
Now things are breaking and I may have reinstall some things, once again for the sake of security.
Ahhhh... where's the balance?


### Day 75: December 11, 2018
**Today's Progress**:
Finished Chapter 11, TDD OTTG book.

**Thoughts**:
Struggled with some minor unix commands and setting up links.
Very good practice to follow along these projects and reproduce.

I certainly am going to be using this deployment recipe again with Fabric.

**Link(s)**
1. [Going to watch/read later - python deployments](https://hynek.me/talks/python-deployments/)
2. [git-based fabric deploys are awesome](http://dan.bravender.net/2012/5/11/git-based_fabric_deploys_are_awesome.html)
3. [I WILL ACTUALLY MEMORIZE THIS - 12 Factor App](https://12factor.net/)


### Day 76: December 12, 2018
**Today's Progress**:
Working on chapter 13 of TDD book.

Was successful at separating tests into files.

**Thoughts**:
Keep looking at remote DevOps jobs.
I found one that really excited me.
Still have to level up a few levels (I feel).

I'll get there.


### Day 77: Decemebr 14, 2018
**Today's Progress**:
Finished chapter 12 of TDD book.

**Thoughts**:
Little hectic today.
Starbucks for day job, couch for fun nerdery.

Quite a bit of screen time and sitting on my ass for one day.


### Day 78: December 15, 2018
**Today's Progress**:
Working through Chapter 13.
Very tired for this late night coding session.

**Thoughts**:
Jerry Maguire was quite the movie. I don't know why I'm thinking through that plot now.
I miss the old Renée Zellweger. :(


### Day 79: December 18, 2018
**Today's Progress**:
Well what happened?

I guess although I did some coding the last two days I did not log it...grrrr.

Tonight I did some coding at Timmies'.

Ahh the wifi always seems to kick me off after an hour use.

Chapter 13 still (i think ) of the TDD book.


### Day 80: December 19, 2018
**Today's Progress**:
Finished chapter 13.
Digging deeper into the code.

**Thoughts**:
* Django community, plenty of opportunity to contribute and join organization 

**Link(s)**
1. [Django Community](https://www.djangoproject.com/community/)


### Day 81: December 20, 2018
**Today's Progress**:
Chewed a little bit through chapter 14 TDD OTTG book

**Thoughts**:
Lazy and holiday mode.


### Day 82: December 21, 2018
**Today's Progress**:
Moving through chapter 14 still of TDD OTTG book.

**Thoughts**:
Q.T. with the S.O. now.


### Day 83: December 22, 2018
**Today's Progress**:
Almost done chapter 14 of TDD OTTD book, after a solid hour I'm now playing "Bird Box" with Sandra Bullocks in the background on Netflix. So far me like.

**Thoughts**:
This TDD books is INTENSE! I feel at time I'm just copying code and have to keep searching back through my kindle version to find the reference of an earlier mentioned function or method. A bit of a pain the arse. I'm sure a hardcopy would be a nightmare is some regards.

For my next challenge of taking on "2 Scoops of Django" that's been sitting on my the shelf for awhile now... I'll see if I dig the paper format I can markup like back in college more than Kindle books.

**Link(s)**
1. [Two Scoops of Django 1.11](https://www.amazon.com/Two-Scoops-Django-1-11-Practices/dp/0692915729)
2. [Update for Shelf dust](https://github.com/twoscoops/two-scoops-of-django-2.0-code-examples)


### Day 84: January 3, 2019
**Today's Progress**:

Back to a proper coding session.

TDD book chapter 15.

Had to dig deep into what *args, and **kwargs were all about. Found a decent site that steps through with a video. I did have to put on the closed captions because he was a fast talker and first time I've heard the word "tuple" besides just reading it.

**Thoughts**:

I'm certainly bumping up against things I'm such a noob at. Today I spent some time thinging about returning to school part-time maybe full time(?) in 2020, to receive my Undergrad degree ontop of my Diploma. I would have to calculate if the cost and time would be worth it... but it's interesting that Lakehead partnership with Georgian has that option.

Youtube sucked me in and I stumbled on the hardware repair video of my GPU panic issue for my MBP Mid2010. What really impressed me about the content creator, Louis Rossmann, is the workshop setup and his casual walk through. The microscope use is something that never occured to me for electronic repairs. I have occassionally repaired iphones in the past and it's becoming a nightmare with my old eyes.


**Link(s)**
1. [GoDjango - *args and **kwargs](https://godjango.com/105-understanding-args-and-kwargs/)
2. [My MBP GPU panic hardware repair](https://www.youtube.com/watch?v=DzcgT_fiVTA)
3. [MBP Mid2010 Software Workaround](https://github.com/julian-poidevin/MBPMid2010_GPUFix)


### Day 85: February 1, 2019
**Today's Progress**:
Finished TDD OTTG(2nd. ed.) chapter 16.

Some very cool JS testing with QUnit!

**Thoughts**:
Continuing right where I left off, with the "I-don't-give-a-damn-about-consecutive-days-rule-I'm-juggling-shit-and-get-tocoding-when-I-can" 100daycodingchallenge.

**Link(s)**
1. [Jasmine](https://jasmine.github.io/)
2. [Testing with Jasmine](http://it-ebooks.directory/book-1449356370.html)
3. [JS the Good Parts](http://it-ebooks.directory/book-0596517742.html)
4. [Mochajs](https://mochajs.org/)


### Day 86: February  7, 2019 (1:00am)
**Today's Progress**:

Some serious coding in! Yeah!

Working through chapter 18 of TDD OTTG. I was stumped a little on setting up the Google app for email, and thinking maybe the book was getting dated ... HOWEVER... when I finally re-read the warning 

*"If you get an SMTPSenderRefused error message, don’t forget to set the EMAIL_PASSWORD environment variable in the shell that’s running runserver."*

- Percival, Harry J. W.. Test-Driven Development with Python: Obey the Testing Goat: Using Django, Selenium, and JavaScript (Kindle Locations 6843-6844). O'Reilly Media. Kindle Edition. 

That was key! The same damn terminal shell. Gosh!!!

Well I took that answer and threw it up on a dead-end Stackoverflow question that was crickets with some people stumped on the the same problem as me. Meh, if I score a few points that would be neato. To rise to a 1K Stackoverflow overlord is something always to aim for. Maybe I'll be as good as Lyndsey Scott one day! 🤞🤞🤞


**Thoughts**:
**Link(s)**
1. [Lyndsey Scott](https://www.instagram.com/p/BCv2H-RE9b7/?taken-by=science)


### Day 87: February 8-9, 2019
**Today's Progress**:
Distracting session infront of Netflix chewing through cahpter 18 TDD OTTG.

Watched some Bodyguard (by myself), and Shameless (with the wife).

**Thoughts**:
Lyndsey Scott was cool enough to reply back to my tweek.

Keep going and put my nerdery in.


## Day 88: February 12, 2019
**Today's Progress**:
Working through chapter 19 TDD OTTG.

Split the time at the EOD and QT with wifey watching Shameless season 8.


**Thoughts**:
I require some serious Python/Django/TDD nerding up.
Just when I think I grappled something serious, I'm back to forgetting something that appears simple.

### Day 89-91: February 19-21, 2019
**Progress**:
Been nerding it up on a few projects.

Last week I tweaked out my neck/back shoveling snow and combining my son's BD this weekend and Family Day, well it's been some time before I was able to get back into my 100-day challenge.

- Worked more on TDD OTTG 2nd ed., finished up (pretty much) chapter 19... only 7 or so chapters to go!
- Worked on moderating some more on Freecodecamp.org
- Actually working on some curriculm projects on FCC as well

**Thoughts**:
Bouncing around is making my learning process a little broad rather than focused.

Excited and a little nervous about the Chingu Voyage 8 starting up tomorrow and juggling the rest of life around that experience.

I actually forgot I enrolled and now I'm getting really excited things are about to start.

Whatever happens I'm really hoping to work on some new Front End, ie. React... and basically working on a development project remotely. It will certainly be different from my day job.

Tonight I had a nice video talk with a fellow moderator, and superstar, that's working on freecodecamp. I always feel I have so much to catch up on.

**Link(s)**
1. [Chingu](https://chingu.io/)


### Day 92-93: February 23, 2019
**Progress**:
Yesterday jumped head first into my Chingu solo pre-work assignment. Have approximately ~~9~~ 8 Days and 13 hours.

I've decided to take on Tier-2 project, using React front-end to build a food drive app to assist people with running a food drive.

Will be MVP as a simple form and a graph of the lbs of food they collected. Something similar to the fork graph on this [fundraiser page](http://cfban.convio.net/site/TR?fr_id=1100&pg=entry).

**Details**:

- Heroku hosted (I'm a little familar with and easy to setup)
- Travis CI (took me awhile to figure out the authentication)
- React front-end
- No idea on the data store portion
- no idea how redux or anything else works for that matter

**Thoughts**:
I've been put on a mission with a deadline and I cannot stop thinking about coding!


**Link(s)**
1. [Solo Project Trello Board](https://trello.com/b/MTvszEjs)
2. [Food Drive steps](https://www.barriefoodbank.org/get-involved/run-a-food-drive/)
3. [Food Drive - Heroku](https://food-drive.herokuapp.com/)
4. [Food Drive - Travis CI](https://travis-ci.com/paulywill/food-drive)
5. [Food Drive - GitHub](https://github.com/paulywill/food-drive)


### Day 94: February 24, 2019
**Today's Progress**:

Stuck on React component elements.

Not sure what to glue everything together let alone use the state and add redux... or fully comprehend what it does.

Time to do some reading and StackOverflow overdrive.

**Thoughts**:

Just when I thought there were some shortcuts I'm back to basics.


### Day 95: February 25, 2019
**Today's Progress**:

Some more troubleshooting with the my React app. Started to watch a crash course that's really clearing up some basics.

**Thoughts**:

Head space (not the meditation app, although I'm a fan of that as well) ... is a very important thing.

I was bummed out about a poor decision about my future at work and that unfortunately put me a funk that was hard to shake. I had to take a break, do some QT with the family and get back in the zone.

It did not hurt to watch the movie Lion tonight. I have NOTHING to complain about in life.

**Link(s)**
1. [React Crash Course](https://www.youtube.com/watch?v=sBws8MSXN7A)


### Day 96: February 26, 2019
**Today's Progress**:
Solo-Project
============
React starting to click with me. I'm creating proper components as per that crash course I found yesterday.

Still have to finish watching and learning about routing. But I'm on the right track by removing some html I was hacking in index.html instead of the src directory.

Peer Programming
================
Have some peer programming to do this afternoon. I'm a little nervous as my partner and I had some conflicting and busy schedules.

Should be fun though.

**Thoughts**:

My incessant job searching during working hours and disinterest in my organization is a good indication my nerd soul/bucket is in need of filling up. :P




**Link(s)**
1. [Redirecting in React](https://medium.com/@anneeb/redirecting-in-react-4de5e517354a)


### Day 97-98: February 27-28, 2019
**Progress**:

Finished the codewar problem that my peer-programmer were working on yesterday. It was some ugly code, and after submitting I looked about some other submission and saw a much more elegent solution via ES6 functions. *Mind-blown*

I was struggling with the a few test cases in codewars because I was using [repl.it](repl.it) and it was picking up some hidden chars or something wacky. In the end our code got the job done. 

Also hacked a little more on my solo-project. Some of the piece still need tweaking. I just a few minutes from finishing that React crash course and grabbed enough concepts to finish I believe.

The "hook" or feature I really wanted to focus my energy on was the "food raised graphic".
So far I have a SVG image of fork-plate-knife; some progress bars available from loading.io; and some half finished CSS and html that's going to line my parts up. 

It's hacky... but I want my MVP to be as convincing and clear as possible.

Will refactor once I understand more about SVG and loading.io libraries.


**Thoughts**:

I once saw, without calling attending to the specific tweet, that someone part taking in the #100daysofcode was enraged that someone could use a day within this challenge to "watch a YouTube video". To which I wanted to say, "GFY!".

Tonight alone I learn so much again from YouTube clip... in fact I'm so impressed with the [creator](http://www.traversymedia.com/), I'm probably going to watch more of his content.

In addition during "a break" I also learn about OnionShare... a file sharing tool for the darkweb that journalists can use to exchange files. That was a random stumble on Twitter.

Random bits of nerdery and ninja is built from learning from others, rather than diving right in head first (without checking how deep the water is).

</rant-over>


**Link(s)**
1. [loading.io](https://loading.io/progress/)
2. [Traversy Media](http://www.traversymedia.com/)
3. [dont be evil - onionshare](https://onionshare.org/)
4. [codewars - paulywill](https://www.codewars.com/users/paulywill/completed)
5. [mirroring cipher - our solution](https://www.codewars.com/kata/reviews/57423abacd764ab93700014f/groups/5c76f24057aa050001892127)
6. [mirroring cipher - best solution](https://www.codewars.com/kata/reviews/57423abacd764ab93700014f/groups/5752b13223b632508500098e)


### Day 99-100: March 2, 2019
**Progress**:

Drained.

Still piecing together my solo-project for chingu :/

Been a solid two days in a row and although I have everything "working" to a presentable level.. there's so much functionality missing.


**Thoughts**:

I was fixated on styling rather than function... I suppose because I could see immediate results. Still getting a grasp on React and this was quite the ambitious undertaking... if they don't accept me to the next level or if I don't finished... I will be a bit bummed... but I've honestly learned a ton already.

I WILL finish though!

oh... and that's 100 days. Yeah!
On to 101...



### Day R2D2: March Day, 2019
**Today's Progress**:

Finished solo-pre work project.


**Thoughts**:

Drained. Absolutly on the verge of tears and divorce last night.
Learned that I had speant the whole time working on the wrong project the entire time.

It's been non-stop hacking and coding since yesterday evening getting a whole new project up and running.

Last night trying to get to sleep was brutal.

Thankfully everything is resolved.

**Link(s)**
1. [paulywill-books](https://paulywill-books.herokuapp.com/)

-------------------------------

### Day xx: Month Day, 2019
**Today's Progress**:
**Thoughts**:
**Link(s)**
1. []()
-------------------------------
