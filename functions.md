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
##foo
