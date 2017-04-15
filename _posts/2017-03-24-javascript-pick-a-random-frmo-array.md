---
layout: post
title: Pick a random value from JavaScript arrays
tags: JavaScript Technology
---
Let's say you want to pick a random value out an array. You can do that in vanilla JavaScript or using any utility libraries like Lodash or Underscore.

Example array

```javascript
var fruitList = ['Apple', 'Mango', 'Banana', 'Orange'];
```
### vanilla JavaScript

Find the length of the array and use Math.random() to pick a value. Math.floor() will help you to pick an integer close to the random number.

```javascript
var randomFruit = fruitList[Math.floor(Math.random() * fruitList.length)];
```

### Underscore

You can use _.sample to pick a random sample from an array. You can also pass an extra parameter to tell the number of random value you need.

Will return one random value
```javascript
_.sample(fruitList);
```

Will return two random values

```javascript
_.sample(fruitList, 2);
```

### Lodash

Similar to Underscore. But called as sampleSize

```javascript
_.sampleSize(fruitList, 2);
```
