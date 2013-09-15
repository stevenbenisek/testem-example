# testem-example

Example [Testem](https://github.com/airportyh/testem) setup using a custom test page. 
Unit testing framework dependencies are installed through [Bower](http://bower.io/). 

## Custom route

Using a custom route the test page is served as a top-level url although it lives in the test folder.

``` json
"routes": {
    "/test.mustache": "test/test.mustache"
}
```

## Dynamic substitution

All source files referenced in `testem.json` are [dynamically inserted](https://github.com/airportyh/testem#dynamic-substitution) in the test page.

``` json
"src_files": [
    "./src/**/*.js",
    "./test/**/*.js"
]
```
