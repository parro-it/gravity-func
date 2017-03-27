# gravity-func

> functional utility for gravity

## Motivation and future directions.

I started this just to learn gravity, and I published it on github
in the hope it can serve as a learning tool for the community.

It' my intention to implement, apart from the exiting `map` and
`filter` function, the following ones:

* [ ] curry
* [ ] reduce
* [ ] compose
* [ ] pipe
* [ ] reverseArgs

## Installation

1) Make sure you have installed and compiled [gravity](https://github.com/marcobambini/gravity):

```bash
    git clone https://github.com/marcobambini/gravity.git
    cd gravity
    make
```

2) Clone this repo under your project directory:

```bash
    git clone https://github.com/parro-it/gravity-func.git packages/gravity-func
```

You can #include this package using `#include` in your project source code:

```
    #include 'packages/gravity-func.gravity'
```

## API

> `func map(fn, data)`

The map() method creates a new array with the results of calling a provided function on every element in this array.

* fn: function that produces an element of the new array, taking two arguments:

    * item - The current element being processed in the array.
    * idx - The index of the current element being processed in the array.

* data: The array map was called upon.

> `func filter(fn, data)`

The filter() method creates a new array with all elements that pass the test implemented by the provided function.

* fn: a predicate, to test each element of the array. Return true to keep the element, false otherwise, taking two arguments:
    * item - The current element being processed in the array.
    * idx - The index of the current element being processed in the array.

* array: The array filter was called upon.

## License

MIT © 2017 Andrea Parodi
