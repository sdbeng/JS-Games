#Exercises
##1 Looping a triangle

Write a loop that makes seven calls to console.log to output the following triangle:
```
#
##
###
####
#####
######
#######
```
my_solution:
```
var t = 6;
var hash = "";
for(var i=0; i<=t; i++){
  hash = hash + "#";
  console.log(hash);
}
```
##2 FizzBuzz

Write a program that uses console.log to print all the numbers from 1 to 100, with two exceptions. For numbers divisible by 3, print "Fizz" instead of the number, and for numbers divisible by 5 (and not 3), print "Buzz" instead.

When you have that working, modify your program to print "FizzBuzz" for numbers that are divisible by both 3 and 5.

**This is actually an interview question that has been claimed to weed out a significant percentage of programmer candidates.**
-Will do step by step: first print numbers from 1-100
```
var n = 0;
var c = 99;
for(var i=0; i <= c; i++){
  n = i + 1;
  console.log(n);
}
```
Next step: with exception1: divisible by 3 and divisible by 5 (not by 3).
```
var n = 0;
var c = 99;
for(var i=0; i <= c; i++){
  	n = i + 1;

	if (n%3 == 0) {
		console.log("Fizz");
	}else if (n%5 == 0 && n%3 != 0) {
		console.log("Buzz");
	}else{
		console.log(n);
	}

}
```
Last step: with exception2: dibisible by 3 and 5.
```
var w
```
If finished, thanks Jesus!
