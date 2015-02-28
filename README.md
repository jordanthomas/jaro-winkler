# Jaro-Winkler

A string similarity function using the Jaro-Winkler distance metric. Returns a
number between 0 and 1. A 0 being no similarity and a 1 being an exact match.

Read more about it [on Wikipedia](http://en.wikipedia.org/wiki/Jaro–Winkler_distance).

## Install

Install in your Node project using npm as usual; `npm install jaro-winkler`. It
also works in the browser, just include the source within `index.js` in your
project however you prefer. Note that the `distance` function will be added to
the global scope if it's not included with a tool lke Browserify.

## Example Usage

```
var distance = require('jaro-winkler');

distance('MARTHA', 'MARHTA');
// 0.961

distance('DWAYNE', 'DUANE');
// 0.84

distance('DIXON', 'DICKSONX');
// 0.814


// Case Insensitive

distance('MARTHA', 'MARTHA');
// 1

distance('mArThA', 'MaRtHa', { caseSensitive: false });
// 1
```
