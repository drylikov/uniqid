# Uniqid.

A super simple, lightning fast unique id based on the current timestamp in milliseconds, with optional prefix and suffix.

## Install

```
$ npm install @drylikov/uniqid
```

## Usage

```js
var uniqid = require("@drylikov/uniqid");

uniqid();
//=> "1558604880081" //string

uniqid('hello-');
//=> "hello-1558604880081" //string

uniqid('', '-world');
//=> "1558604880081-world" //string

uniqid('hello-', '-world');
//=> "hello-1558604880081-world" //string

```


### Options


|            Name          |                  Type                       | Default Value |
|--------------------------|---------------------------------------------|---------------|
| prefix                   | String                                      |       ''      |
| suffix                   | String                                      |       ''      |