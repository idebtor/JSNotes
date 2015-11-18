# replace()

    str.replace(regexp|substr, newSubStr|function[, flags])
    
[reference for replace](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)

[reference for regexp](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp)

## Example 1:
In the following example, the regular expression is defined in replace() and includes the ignore case flag.

    var str = 'Twas the night before Xmas...';
    var newstr = str.replace(/xmas/i, 'Christmas');
    console.log(newstr);  // Twas the night before Christmas...

## Example 2:
In the following example, the regular expression includes the global and ignore case flags which permits replace() to replace each occurrence of 'au' in the string with 'U'.

    var s = "audacity audacity";
    var udacityizer = function(s) {  
    // Right now, the variable s == "audacity audacity"
        return s.replace(/au/gi, 'U'); // return "Udacity Udacity"
    };

## Example 3:
In the following example, the function returns true if the given string is a palindrome. Otherwise, return false. You'll need to remove punctuation and ignore cases. A palindrome is a word or sentence that's spelled the same way both forward and backward, ignoring punctuation, case, and spacing.

```
function palindrome(str) {
  str = str.replace(/[^a-zA-Z0-9]+/gi, '').toLowerCase();
  return str == str.split('').reverse().join('');
}

// examples of palindrome 
palindrome("eye");
palindrome("Race car");
palindrome("Never odd or even");
palindrome("0_0 (: /-\ :) 0-0");
```

## Example 4:
In the following example, the function returns the string that does not contain any < or >. 

var html = '<script src="http://hackyourwebsite.com/eviljavascript.js"></script>';
var charEscape = function(_html) {
    return _html.replace(/[<>]/gi, '');
};

// Did your code work? The line below will tell you!
console.log(charEscape(html));
