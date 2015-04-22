# Ice for JavaScript

[Ice](https://github.com/zeroc-ice/ice) is a comprehensive RPC framework with support for C++, .NET, Java, Python, JavaScript and more. This repository contains the [bower](http://bower.io/) distribution of Ice for JavaScript.

## Install

```bash
$ bower install ice --save
```

## Usage

Add the necessary `<script>` tags to your html to include the Ice for JavaScript components you require.

```html
<script src="/bower_components/ice/lib/Ice.js"></script>
<script src="/bower_components/ice/lib/Glacier2.js"></script>
<script src="/bower_components/ice/lib/IceStorm.js"></script>
<script src="/bower_components/ice/lib/IceGrid.js"></script>
<script type="text/javascript">
    var communicator = Ice.initialize();
    var proxy = communicator.stringToProxy("hello:ws -h localhost -p 10002");
</script>
```

Minified versions are available with the `.min.js` extension.

## Documentation

See the [Ice Documentation](https://doc.zeroc.com/display/Ice36/JavaScript+Mapping).

## Slice2js Compiler

To compile [Slice](https://doc.zeroc.com/display/Ice36/The+Slice+Language) files to JavaScript see the following:
- [slice2js](https://github.com/zeroc-ice/npm-slice2js)
- [gulp-ice-builder](https://github.com/zeroc-ice/gulp-ice-builder)

## Demos

A collection of demos for Ice for JavaScript (and other language mappings) can be found [here](https://github.com/zeroc-ice/ice-demos).
