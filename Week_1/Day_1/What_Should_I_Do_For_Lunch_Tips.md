### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.


```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  //check the hungry boolean, if not hungry time available does not matter
  if (hungry === true) {

    //checking available time to give appropriate response
    if (availableTime < 20) {
      console.log("I should pick something up and eat while working");
    } else if (availableTime >= 20 && availableTime < 30) {
      console.log("Let's try a local resteraunt or a cafe");
    } else {
      console.log("I have a lot of work to do and probably shouldn't spend that much time on lunch");
    }
  } else {
    //if not hungry keep working
    console.log("I should keep working until I'm hungry");
  }
};
```