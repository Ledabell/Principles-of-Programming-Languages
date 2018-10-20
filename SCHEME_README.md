# Scheme Project 

This is a description of the Scheme project. We can us the given functions to evaluate buckets of colored balls and judge which one has the highest point value.

* The main feature is the judge function used to find the best of two buckets.
* You can also use the other 4 functions to find out more info about each individual bucket.

### Quick start
**Make sure you have the latest version of DrRacket downloaded.

> Clone/Download the solution then run `funfair_scheme.rkt`

```

# Download all files from canvas

# For Mac OSX
Open funfair_scheme.rkt in DrRacket and hit run at the top right. Enter in function calls as desired.

```

# Table of Contents
* [Scheme chapter](#scheme-chapter)
* [API Intro](#api-intro)
* [Implementation](#implementation)
* [API Intro](#api-intro)
* [Time Complexity](#time-complexity)
* [Sample Test Case](#sample-test-case)
* [License](#license)
* [Author](#author)

#### Scheme chapter

For this project we used Scheme to provide 5 different functions that allow the user to evaluate different buckets to get information about them as well as compare buckets to each other.

___

#### API Intro

The following are the 5 functions provided in this program: 

```
(define (ball-val ball)
.
.
)
```

The ball-val function takes one argument, a ball of some color, and returns the point value of that ball.

Sample usage:
> (ball-val 'R)
10

```
(define (count-balls ball bucket)
.
.
)
```

The count-balls function takes two arguments, a ball of some color and a bucket. The function counts the number of that color ball in the given bucket and returns that number.

Sample usage:
> (count-balls 'R '(R B G R R R B W R W))
5

```
(define (color-counts bucket)
.
.
)
```

The color-counts funtion takes one argument, a bucket containing colored balls. The function evaluates home many of each color ball are in the bucket and returns it in a list of order (Red Green Blue White).

Sample usage:
> (color-counts '(R B G R R R B W R W))
'(5 1 2 2)

```
(define (bucket-val bucket)
.
.
)
```

The bucket-val function takes one argument, a bucket containing colored balls. The function calculates the total point value of the bucket by adding up the points for each ball in the bucket, and returns that value.

Sample usage:
> (bucket-val '(R B G R R R B W R W))
107

```
(define (judge bucket_1 bucket_2)
.
.
)
```

The judge function takes two arguments, two buckets containing colored balls. The function gets each bucket's total point value and compares them to see which wins or if they are tied and returns the result.

Sample usage:
> (judge '(R B G R R R B W R W) '(W R R R R G B B G W))
Bucket 2 Won!
___

#### Implementation

The program uses a lambda function to count the balls of a certain type and uses lists to return how many of each ball color there are for a given bucket. This maintains efficiency and readability of the code.

___

#### Time Complexity

The program runs with O(n) time complexity.

___

#### Sample Test Case

some image or output is shown by Foo program execution......

___

#### License
 [Auburn University](/LICENSE)

___

## Author
 [Aleha Crumpton](/LICENSE)
