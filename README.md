# Web API with Vanilla JS

This is a quick example of how to use vanilla JavaScript to display information from a web API. The example uses the [Google Books API, version 1](https://developers.google.com/books/docs/overview).

You can easily replace the actual API call to a different service and then backwards engineer the markup based on the new data that's returned.

## Browser Support

### Polyfills

This example is using the [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) which is based on the [Promise object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) and is supported by all modern browsers, [except Internet Explorer and older mobile browsers](https://caniuse.com/#search=fetch). If you want to provide support for those browsers you can add polyfills for the Promise object and the Fetch API:

* [Promise() Polyfill](https://vanillajstoolkit.com/polyfills/promise/) (Pushes support back to IE9)
* [fetch() Polyfill](https://vanillajstoolkit.com/polyfills/fetch/) (Pushes support back to IE10)

You can also use the [Polyfill.io](https://polyfill.io/v3/) service in order to automate this process.

### ES6 Syntax

The [ES6 template literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals) used in the example make it easier to add JSON data into a string, but are [not supported in Internet Explorer and some mobile browsers](https://caniuse.com/#search=template%20literals).

To add support for ES6 syntax such as template literals, you must transpile the code to ES5 syntax using a compiler tool like [Babel](https://babeljs.io/repl).
