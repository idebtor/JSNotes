# What is JSON?

**J**ava**S**cript **O**bject **N**otation. JSON is a popular and simple format for storing and transferring nested or hierarchal data. It's so popular that most other programming languages have libraries capable of parsing and writing JSON (like Python's JSON library). Internet GET and POST requests frequently pass data in JSON format. JSON allows for objects (or data of other types) to be easily encapsulated within other objects. See the [JSON.org](http://json.org/) for more details.

# Why should I lint my JSON?
With a mix of nested curly braces, square brackets and commas, it's easy to make mistakes with JSON. And mistakes mean bugs, seriously.  If you're generating JSON by hand, you should copy and paste your code into a JSON linter like [jsonlint.com](http://jsonlint.com/) to quickly and easily find syntax errors. A linter is a piece of software that analyzes code for syntax errors. Some text editors, like Sublime Text, will automatically lint (or highlight) most syntax errors. But a JSON linter won't miss any syntax errors and you can rest assured that your JSONs will be properly formatted.

**Tip:** jsonlint.com works for one object only.

# An Example:
In the following example, 

    1. Cut from the fist '{' to last '}'.
    2. Paste it on the panel(window) displayed by jsonlint.com. 
    3. Click 'validate'.
    4. Fix your object as needed. 

```
 var education = {
     "schools": [
         {
             "name": "Emory University", 
             "city": "Atlanta",
             "majors": ["EE"],
             "minor": "Bio",
             "classYear": 2000
         },
         {
             "name": "Chicago College", 
             "city": "Chicago",
             "majors": ["Economics"],
             "minor": "Chemistry",
             "classYear": 2005             
         }
     ],
    "onlineCourses": [
        {
            "title": "JavaScript", 
            "school": "Udacity",
            "dates": 2015,
            "url": "http://www.udacity.com/course/ud804"
        }
    ]
}
```

