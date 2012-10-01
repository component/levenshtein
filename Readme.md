
# levenshtein
## The "[Levenshtein Distance][wiki]" algorithm

The "Levenshtein Distance" algorithm is a "string metric" for mesuring the
similarity between two Strings.

It returns a Number from `0-Infinity`. The lower the number, the closer the two
strings are to being equal.

### Example

``` js
var levenshtein = require('levenshtein');

console.log(levenshtein('Nathan Rajlich', 'Nathan Rajlich'));
// 0

console.log(levenshtein('Nathan Rajlich', 'nathan rajlich'));
// 2

console.log(levenshtein('Nathan Rajlich', 'nathanrajlich'));
// 3

console.log(levenshtein('Nathan Rajlich', 'TJ Holowaychuk'));
// 13
```

[wiki]: http://wikipedia.org/wiki/Levenshtein_distance
