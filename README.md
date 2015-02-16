# Jaro-Winkler

A string similarity function using the Jaro-Winkler distance metric. Returns a
number between 0 and 1. A 0 being no similarity and a 1 being an exact match.

Read more about it [on Wikipedia](http://en.wikipedia.org/wiki/Jaro–Winkler_distance).

## Install

```
npm install jaro-winkler
```

## Usage Examples

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
