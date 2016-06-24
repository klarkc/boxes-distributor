boxes-distributor
=

[![Travis][travis-image]][travis-url]

[travis-image]: https://img.shields.io/travis/klarkc/boxes-distributor/master.svg
[travis-url]: https://travis-ci.org/klarkc/boxes-distributor

This element try to organize boxes in a truck in the most efficient layout. Example:

```
Bad layout example:

           300
x-------------------------x
|         |         |     |              
|         |         |     |
|  54x42  |  54x42  |     | 192
|         |         |     |     
|         |         |     |          
x-------------------------x

Total: 2 boxes


Good layout example!

           300
x-------------------------x
|         |               |
|         |     42x54     |
|  54x42  |---------------| 192
|         |     42x54     |
|         |               |
x-------------------------x

Total: 3 boxes

```

Demo and API: https://klarkc.github.io/boxes-distributor/

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install


## Playing With Your Element

If you wish to work on your element in isolation, we recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve

Once running, you can preview your element at
`http://localhost:8080/components/boxes-distributor/`, where `boxes-distributor` is the name of the directory containing it.


## Testing Your Element

Simply navigate to the `/test` directory of your element to run its tests. If
you are using Polyserve: `http://localhost:8080/components/boxes-distributor/test/`

### web-component-tester

The tests are compatible with [web-component-tester](https://github.com/Polymer/web-component-tester).
Install it via:

    npm install -g web-component-tester

Then, you can run your tests on _all_ of your local browsers via:

    wct

#### WCT Tips

`wct -l chrome` will only run tests in chrome.

`wct -p` will keep the browsers alive after test runs (refresh to re-run).

`wct test/some-file.html` will test only the files you specify.


## Yeoman support

If you'd like to use Yeoman to scaffold your element that's possible. The official [`generator-polymer`](https://github.com/yeoman/generator-polymer) generator has a [`seed`](https://github.com/yeoman/generator-polymer#seed) subgenerator.
