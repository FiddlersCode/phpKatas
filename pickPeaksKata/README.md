# Pick Peaks Kata
by Paula Muldoon 

### About
This kata is taken from [CodeWars](https://www.codewars.com/kata/pick-peaks). I have modified the instructions to make them clearer.

### The Brief
In this kata, you will write a function that returns the position and the value of the [local maxima](https://en.wikipedia.org/wiki/Maxima_and_minima), here defined as "peaks", of a numeric array.

#### Specs
- The output will be returned as an associative array with two key-value pairs: `'pos'` and `'peaks'`. 
- Each value should be a non-associative array. 
- All input arrays will be valid integer arrays (although they could be empty), so you won't need to validate the input.
- The first and last elements of the array will **not** be considered peaks (mathematically, as we don't know what is before or after we can't know if it is a peak).
- In case of a plateau peak, return the position and value of the beginning of the plateau. 
- If there is no peak in the given array, simply return `['pos' => [], 'peaks' => []]`.


#### Examples
- `arr = [0, 1, 2, 5, 1, 0]` has a peak at position 3 with a value of 5 (since `arr[3] equals 5`).
- `pickPeaks([3, 2, 3, 6, 4, 1, 2, 3, 2, 1, 2, 3])` should return `{pos: [3, 7], peaks: [6, 3]}`.
- `[1, 2, 2, 2, 1]` has a peak while `[1, 2, 2, 2, 3]` does not.
- `pickPeaks([1, 2, 2, 2, 1])` returns `{pos: [1], peaks: [2]}`

Have fun!

### To run

- Run `composer init` and create the `composer.json` file
- Run `composer install`
- To run tests: `phpunit tests`
```bash
phpunit tests
```

### Processes
* TDD


### Technologies used

* [PHP 5.6.3](http://www.php.net/)
* [PHPUnit 5.7.21](https://phpunit.de/)

