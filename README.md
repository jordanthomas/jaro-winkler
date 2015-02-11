# jaro-winkler
A string similarity function using the Jaro-Winkler distance metric.

## Install

```
npm install jaro-winkler
```

## Basic Usage

```
var distance = require('jaro-winkler');

distance('MARTHA', 'MARHTA');
// 0.961

distance('DWAYNE', 'DUANE');
// 0.84

distance('DIXON', 'DICKSONX');
// 0.814
```
