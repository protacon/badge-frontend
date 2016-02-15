# What is this?
[![License](http://img.shields.io/:license-mit-blue.svg)](LICENSE)
[![GitHub version](https://badge.fury.io/gh/ProtaconSolutions%2Fbadge-frontend.svg)](https://badge.fury.io/gh/ProtaconSolutions%2Fbadge-frontend)
[![Dependency Status](https://david-dm.org/ProtaconSolutions/badge-frontend.svg)](https://david-dm.org/ProtaconSolutions/badge-frontend)
[![devDependency Status](https://david-dm.org/ProtaconSolutions/badge-frontend/dev-status.svg)](https://david-dm.org/ProtaconSolutions/badge-frontend#info=devDependencies)

Badge frontend application which uses [AngularJS](https://angularjs.org/). 
This frontend uses [badge-backend](https://github.com/ProtaconSolutions/badge-backend).

## Main points
- [x] Gulp task to help development process
- [ ] Build / deploy process
- [ ] Material design
- [ ] Configuration for each environment and/or developer
- [ ] Configuration for each environment and/or developer
- [ ] And all the _rest_

## Requirements

## Installation
First of all you have to install ```npm``` and ```node.js``` to your box. Installation instructions can
be found [here](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager).

After that you need to install ```bower``` and ```gulp<``` main packages to make all  things to happen. 
These can be installed with following commands on your *nix box. 
```
sudo npm install bower -g
sudo npm install gulp -g
```

And when you have ```npm``` and ```node.js``` installed to your box, just navigate yourself to root folder
of the app and run following commands:

```
npm install
```

### Configuration
See ```/src/app/config/config.json_example``` file and copy it to ```/src/app/config/config.json``` file and make
necessary changes to it. 

## Development

To start developing in the project run:

```bash
gulp serve
```

Then head to `http://localhost:3000` in your browser.

The `serve` tasks starts a static file server, which serves the AngularJS application, and a watch task which watches 
all files for changes and lints, builds and injects them into the index.html accordingly.

## Production ready build - a.k.a. dist

To make the app ready for deploy to production run:

```bash
gulp dist
```

Now there's a `./dist` folder with all scripts and stylesheets concatenated and minified, also third party libraries 
installed with bower will be concatenated and minified into `vendors.min.js` and `vendors.min.css` respectively.

### Running production ready build

To start production ready build in the project run:

```bash
gulp production
```

Then head to `http://localhost:3001` in your browser

## Contributing
Please see the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines.

## Author
[Tarmo Leppänen](https://github.com/tarlepp)

## LICENSE

[The MIT License (MIT)](LICENSE)

Copyright (c) 2016 Protacon Solutions