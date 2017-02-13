# jsdoc-plugin-abitbol

A jsdoc plugin which simplifies [abitbol](https://github.com/wanadev/abitbol) classes documentation.

## Installation

Install `jsdoc-plugin-abitbol`

```shell
npm install --save-dev jsdoc-plugin-abitbol
```

Add an entry in the `plugins` list of your `jsdoc` config file :

```json
{
    "plugins": ["node_modules/jsdoc-plugin-abitbol"]
}
```

## Usage

```js
const MyClass = Class.$extend({
    /**
     * My class.
     *
     * @class namespace.MyClass
     * @extends Class
     * @param params {Object} The parameters.
     */
    __init__(params) {
        // ...
    },

    /**
     * The name.
     *
     * @member name
     * @type {String}
     * @default null
     */
    getName() {
        // ...
    },
    setName(name) {
        // ...
    },

    /**
     * My method.
     *
     * @param {Object} params The parameters.
     * @return {String} The result.
     */
    method1(params) {
        // ...
    },
}
```
