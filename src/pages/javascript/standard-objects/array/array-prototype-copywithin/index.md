## Array.prototype.copyWithin
The ``copyWithin()`` method overwrites part of the array with another part of it. This method **both modifies and returns** the array.

It can take **2 or 3 inputs**:
* 2 inputs: ``copyWithin(overwriteFromHere, copyFromHereToEnd)``
* 3 inputs: ``copyWithin(overwriteFromHere, copyFromHere, copyToHere)``

**Examples**
```javascript
var letters = ["a", "b", "c", "d", "e", "f", "g"]

// 2 inputs
console.log(letters.copyWithin(1, 4)) // items(everything after 4) 4-5-6 to position 1-2-3(after 1)
                                      // ["a", "e", "f", "g", "e", "f", "g"]
                                      
// 3 inputs
letters = ["a", "b", "c", "d", "e", "f", "g"]
console.log(letters.copyWithin(1, 4, 6)) // items(everything between 4 and 6) 4-5 to position 1-2(after 1)
                                         // ["a", "e", "f", "d", "e", "f", "g"]
```
