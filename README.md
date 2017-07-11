# eslint-plugin-jsdoc-lazy

Apply the eslint rule `require-jsdoc`, but prevent reporting for special class methods and react lifecycle methods.

## Installation

You'll first need to install [ESLint](http://eslint.org):

```
$ npm i eslint --save-dev
```

Next, install `eslint-plugin-jsdoc-lazy`:

```
$ npm install eslint-plugin-jsdoc-lazy --save-dev
```

**Note:** If you installed ESLint globally (using the `-g` flag) then you must also install `eslint-plugin-jsdoc-lazy` globally.

## Usage

Add `jsdoc-lazy` to the plugins section of your `.eslintrc` configuration file. You can omit the `eslint-plugin-` prefix:

```json
{
    "plugins": [
        "jsdoc-lazy"
    ]
}
```


Then configure the rules you want to use under the rules section.

```json
{
    "rules": {
        "jsdoc-lazy/rule-name": 2
    }
}
```

## Supported Rules

```require-jsdoc``` - includes the original eslint rule, but ignores:

    'constructor',
    'render',
    'componentWillMount',
    'componentDidMount',
    'componentWillUnmount',
    'shouldComponentUpdate',
    'componentWillUpdate',
    'componentDidUpdate'





