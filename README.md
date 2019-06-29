# Loops Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**

***

var numBer = 1

while numBer <= 150 {
print(numBer)
numBer+=1
}


## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

***

let value = 142...149
var i = 0

for _ in 142..<159 {
print(i)
i += 1
}

## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

***

let aRange = 15...80

for evenNumbers in aRange where evenNumbers % 2 == 0 {
print(evenNumbers)
}

## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

***

let aRange = 19...51

for oddNumbers in aRange where oddNumbers % 2 != 0 {
print(oddNumbers)
}

## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

***

let aRange = 1...100

for i in aRange where i % 10 == 5 {
print(i)
}


## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

***

let aRange = 1...40

for i in aRange where i % 10 == 7 {
print(i)
}

## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

***

let aRange = 20...150

for i in 20...150 {
if i % 3 == 0 {
print(i)
}
}

## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

***

let aRange = 20...150

for i in 20...150 {
if (i % 2) && (i % 3) {
print(i)
}
}


## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

***

let aRange = 20..<150

for i in aRange where i % 10 == 4 {
print(i)
}

## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

***

var aRangeOfNumbers = 20...150

for i in aRangeOfNumbers {
if i == 31 || i == 35 || i >= 40 && i <= 60 {
print(i)
}
}

## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

// 

var i = 5

while (i > 3) {
i += 1
}

// Because 5 is not less than 3, it is going up in incriments of the value of i plus 1


***

## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
var i = 5

while (i < 9) {
i += 1
}

***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```

***

var i = 5

while (i > 3) {
i += 1
}

## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i > 3) {
    i += 1
}
```

var i = 0

while (i < 1000) {
i += 1
if i % 2 == 0 {
print(i)
}
}


***
## Question 15

What's the difference in syntax between the following two while loops?  Will their outputs be different?  Explain why or why not.

```swift
var i = 1
//loop one
while i <= 10 {
    print("i = \(i)")
    i += 1
}

//loop two
var i = 1

repeat {
    print("i = \(i)")
    i += 1
} while i <= 10
```
The difference is the repeat function. The loops are the the same because the string interpolation works for both variables.
***
## Question 16

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

***

If there is a break in the code, that means that it is breaking it up just to set it aside for another time. While with continue, you are going in a set of motion until a condition is met.

for i in 1...65 {
if (i >= 5 && i <= 8){
continue
}
print(i)
}


## Question 17

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        continue
    }
    print(i)
}
```

[x]1
[x]2
[x]3
[]4
[]5
[]6
[]7
[x]8
[x]9
[x]10

***
## Question 18

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        break
    }
    print(i)
}
```

[x]1
[x]2
[x]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10

***
## Question 19

Without using Xcode, what will the loop below print?  Explain below.

```swift
outerloop: for x in 1...3 {
    innerloop: for y in 1...3 {
        if y == 2{
            continue outerloop
        }
        print("x = \(x), y = \(y)")
    }
}
```
outerloop: for x in 0...10 {
innerloop: for y in 0...10 {
print("x = \(x), y = \(y)")
}
}

//It checks the if condition when its true, it continues to the outerloop. It never prints the inner loop.

***
## Question 20

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

***

for x in 0...10 {
for y in 0...10 {
print("x = \(x), y = \(y)")
}
}

## Question 21

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

***

var a = 10

for x in 0...a{
for y in 0...a{
if x - y >= 5 {
print("x = \(x), y = \(y)")
}
}
}


## Question 22

Print the first `N` square numbers. A **square number**, also called perfect square, is an integer that is obtained by squaring some other integer; in other words, it is the product of some integer with itself (ex. 1 = 1*1, 4 = 2 * 2, 9 = 3* 3 …).

Example:
Input: `var N = 5`

Output:
```swift
1
4
9
16
25
```
var N = 40
var i = 1

while i<=N {
print(i * i)
i += 1
}


***
## Question 23

Given an integer N draw a square of N x N asterisks. Look at the examples.

Example 1:
Input: `var N = 2`

Output:
```swift
**
**
```

Example 2:
Input: `var N = 3`

Output:
```swift
***
***
***
```

var N = 2
var holder = ""

for _ in 1..<N {
for _ in 1..<N {
holder += *
}
}

***
