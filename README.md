<!--

@license Apache-2.0

Copyright (c) 2022 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# copyIndexed

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Copy the elements of an indexed array-like object to a new "generic" array.

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->



<section class="usage">

## Usage

```javascript
import copyIndexed from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-base-copy-indexed@deno/mod.js';
```

#### copyIndexed( x )

Copies the elements of an indexed array-like object to a new "generic" array.

```javascript
var x = [ 1, 2, 3 ];

var out = copyIndexed( x );
// returns [ 1, 2, 3  ]

var bool = ( out === x );
// returns false
```

</section>

<!-- /.usage -->

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

## Notes

-   An _indexed_ array-like object is a data structure in which one retrieves elements via integer indices using bracket `[]` notation (e.g., `Float64Array`, `Int32Array`, `Array`, etc). This is in contrast to an _accessor_ array-like object in which one retrieves elements using `get` and `set` methods (e.g., `Complex64Array` and `Complex128Array`).

</section>

<!-- /.notes -->

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
import filledBy from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-filled-by@deno/mod.js';
import randu from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-base-randu@deno/mod.js';
import copyIndexed from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-base-copy-indexed@deno/mod.js';

// Create a Float64Array:
var arr = filledBy( 10, 'float64', randu );

// Copy elements to a generic array:
var out = copyIndexed( arr );

// Retrieve the first element:
var x = out[ 0 ];
// returns <number>

console.log( '%d', x );
```

</section>

<!-- /.examples -->

<!-- Section to include cited references. If references are included, add a horizontal rule *before* the section. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="references">

</section>

<!-- /.references -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/array-base-copy-indexed.svg
[npm-url]: https://npmjs.org/package/@stdlib/array-base-copy-indexed

[test-image]: https://github.com/stdlib-js/array-base-copy-indexed/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/array-base-copy-indexed/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/array-base-copy-indexed/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/array-base-copy-indexed?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/array-base-copy-indexed.svg
[dependencies-url]: https://david-dm.org/stdlib-js/array-base-copy-indexed/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/array-base-copy-indexed/tree/deno
[umd-url]: https://github.com/stdlib-js/array-base-copy-indexed/tree/umd
[esm-url]: https://github.com/stdlib-js/array-base-copy-indexed/tree/esm
[branches-url]: https://github.com/stdlib-js/array-base-copy-indexed/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/array-base-copy-indexed/main/LICENSE

</section>

<!-- /.links -->
