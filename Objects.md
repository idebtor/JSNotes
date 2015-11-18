
# Objects, but no classes

In JavaScript object is a collection of name and value pairs. Believe or not, there is no class. JavaScript objects behave a lot like Python dictionaries, but there are some differences. 

- python code:
```
    menu = {}
    menu['Chicken Alfredo'] = 14.50
    menu['Italian Pasta'] = 15.89
    menu['Shrimp Soup'] = 12.43
```    
- javascript code:
```
    var menu = new Object();
    menu['Chicken Alfredo'] = 14.50;
    menu['Italian Pasta'] = 15.89;
    menu['Shrimp Soup'] = 12.43;
```
For a detailed comparison, see [this StackOverflow thread](http://stackoverflow.com/questions/20987485/python-dictionaries-vs-javascript-objects).

Though JavaScript has **no classes**, you can mimic many of the characteristics with its functions. 
```
    function Car() {}
    /*
    var Car = function() {}
    */
    var car1 = new Car();
```    
The new keyword allows us to create a new instance of an Object. Remember that functions are objects. In the code above, you can think of the function Car as a JavaScript version of a Python class definition.
