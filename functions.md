 ##we call the function by name
 Here, it is called 'dividebythree'
We tell the computer what the number input is (i.e. 6)
The computer then runs the code inside the function!

This is what a function looks like:
```
var divideByThree = function (number) {
    var val = number / 3;
    console.log(val);
};
divideByThree(45);
```
We can join strings together using the plus sign (+)

```
var greeting = function (name) {
    console.log("Great to see you," + " " + name);
};

greeting("mom and dad!");
```
## Name changer (capitalizer)

```
function nameChanger(oldName) {
    var finalName = oldName;
    var names = oldName.split(" ");
    names[1] = names[1].toUpperCase();
    names[0] = names[0].slice(0,1).toUpperCase() + names[0].slice(1).toLowerCase();
    finalName = names.join(" ");
    return finalName;
}
```
Explain: giving the param (oldName = "AlbERt EINstEiN") we do this:
var names = oldName.split(" ")

Here, we're creating an array of names by breaking the original name at the space. At this point for our original example, names === ["AlbERt", "EINstEiN"]

names[1] = names[1].toUpperCase();

The string.toUpperCase() method does exactly what its name describes. It's acting on names[1], which is "EINstEiN" in the original example. So here, we're reassigning the second element in the names array to the all caps version of "EINSTEIN".

names[0] = names[0].slice(0,1).toUpperCase() + names[0].slice(1).toLowerCase();

This line builds Albert. names[0].slice(0,1).toUpperCase() starts by acting on the first element in the names array, which is "AlbERt" in the example. Then, we grab just the first letter by using .splice(0,1). Then we simply use the .toUpperCase() method again to make sure the first letter is capitalized. Also, notice how we chained two methods together here.

The next part, names[0].slice(1).toLowerCase() acts similarly, except this time we're using .slice(1) to grab the rest of the first string, which is "lbERt" in the example. Then we simply chain the .toLowerCase() method to make sure that the rest of the letters in the first name are lower case. Once we have the first letter capitalized and the rest of the name lower case, we concatenate them together with the +.

finalName = names.join(" ");

array.join([chars]) lets us put array elements together into a single string. Each element will be separated by the optional chars. In this case, we want a space between the two names, so we made the chars a single space, " ". With that, we've joined "Albert" and "Einstein" to form "Albert EINSTEIN"!

##foo
