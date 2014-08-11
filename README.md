# css-minimizers-bench

Сompares the work of CSS minimizers.

## Which CSS minimizers are compared?

* [CSSO](https://github.com/css/csso)

* [clean-css](https://github.com/GoalSmashers/clean-css)

* [cssshrink](https://github.com/stoyan/cssshrink)

## Install

```bash
$ git clone https://github.com/eGavr/css-minimizers-bench.git

$ cd css-minimizers-bench

$ npm install
```

## Usage

```bash
$ bin/compare-minimizers
```

## How to add your minimizer?

1. Go to the [package.json](https://github.com/eGavr/css-minimizers-bench/blob/master/package.json#L28-L30) and add your minimizer to the dependencies.

2. Go to the [configuration file](https://github.com/eGavr/css-minimizers-bench/blob/master/lib/config.js#L8-L10) and add your code according to the following template:
```js
"name-of-your-minimizer": minimize(require("your-minimizer's module"), "name-of-minimization-method-of-your-minimizer")
```
3. Reinstall dependencies
```bash
npm install
```
4. See [usage](https://github.com/eGavr/css-minimizers-bench#usage).

## License

[MIT License](http://en.wikipedia.org/wiki/MIT_License)
