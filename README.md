<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Archavercosine

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Compute the [inverse half-value versed cosine][archavercosine].

<section class="intro">

The [inverse half-value versed cosine][archavercosine] is defined as

<!-- <equation class="equation" label="eq:archavercosine" align="center" raw="\operatorname{ahavercos}(\theta) = 2 \cdot \arccos(\sqrt{\theta})" alt="Inverse half-value versed cosine."> -->

```math
\mathop{\mathrm{ahavercos}}(\theta) = 2 \cdot \arccos(\sqrt{\theta})
```

<!-- <div class="equation" align="center" data-raw-text="\operatorname{ahavercos}(\theta) = 2 \cdot \arccos(\sqrt{\theta})" data-equation="eq:archavercosine">
    <img src="https://cdn.jsdelivr.net/gh/stdlib-js/stdlib@bb29798906e119fcb2af99e94b60407a270c9b32/lib/node_modules/@stdlib/math/base/special/ahavercos/docs/img/equation_archavercosine.svg" alt="Inverse half-value versed cosine.">
    <br>
</div> -->

<!-- </equation> -->

</section>

<!-- /.intro -->

<section class="installation">

## Installation

```bash
npm install @stdlib/math-base-special-ahavercos
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm` branch][esm-url].
-   If you are using Deno, visit the [`deno` branch][deno-url].
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd` branch][umd-url].

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

</section>

<section class="usage">

## Usage

```javascript
var ahavercos = require( '@stdlib/math-base-special-ahavercos' );
```

#### ahavercos( x )

Computes the [inverse half-value versed cosine][archavercosine].

```javascript
var v = ahavercos( 0.0 );
// returns ~3.1416

v = ahavercos( 1.0 );
// returns 0.0

v = ahavercos( 0.5 );
// returns ~1.5708
```

If `x < 0`, `x > 1`, or `x` is `NaN`, the function returns `NaN`.

```javascript
var v = ahavercos( 1.5 );
// returns NaN

v = ahavercos( -3.14 );
// returns NaN

v = ahavercos( NaN );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var linspace = require( '@stdlib/array-base-linspace' );
var ahavercos = require( '@stdlib/math-base-special-ahavercos' );

var x = linspace( 0.0, 1.0, 100 );

var i;
for ( i = 0; i < x.length; i++ ) {
    console.log( ahavercos( x[ i ] ) );
}
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math-base/special/ahaversin`][@stdlib/math/base/special/ahaversin]</span><span class="delimiter">: </span><span class="description">compute the inverse half-value versed sine.</span>
-   <span class="package-name">[`@stdlib/math-base/special/havercos`][@stdlib/math/base/special/havercos]</span><span class="delimiter">: </span><span class="description">compute the half-value versed cosine.</span>
-   <span class="package-name">[`@stdlib/math-base/special/vercos`][@stdlib/math/base/special/vercos]</span><span class="delimiter">: </span><span class="description">compute the versed cosine.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-ahavercos.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-ahavercos

[test-image]: https://github.com/stdlib-js/math-base-special-ahavercos/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/math-base-special-ahavercos/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-ahavercos/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-ahavercos?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-ahavercos.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-ahavercos/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-ahavercos/tree/deno
[umd-url]: https://github.com/stdlib-js/math-base-special-ahavercos/tree/umd
[esm-url]: https://github.com/stdlib-js/math-base-special-ahavercos/tree/esm
[branches-url]: https://github.com/stdlib-js/math-base-special-ahavercos/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-ahavercos/main/LICENSE

[archavercosine]: https://en.wikipedia.org/wiki/Versine

<!-- <related-links> -->

[@stdlib/math/base/special/ahaversin]: https://github.com/stdlib-js/math-base-special-ahaversin

[@stdlib/math/base/special/havercos]: https://github.com/stdlib-js/math-base-special-havercos

[@stdlib/math/base/special/vercos]: https://github.com/stdlib-js/math-base-special-vercos

<!-- </related-links> -->

</section>

<!-- /.links -->
