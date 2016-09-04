# `Angular2/Webpack/Docker Seed Project`

### Description:
Angular2 RC6 Seed based on **docker-compose** and **webpack** bundler.
Implemented:
- Latest Angular2 Version (RC6)
- Dev/Prod Environments **docker/npm**.
- Webpack **Watch** (detect change, compile, reload browser).
- Component can use **SCSS** directly ex: ```styles: [require('./app.scss')]```
- **Code Style checker** and TS/JS Linters.
- Src, Vendor and Pollyfills are split into 3 files.
Coming Soon:
- Jasmin and Karma tests.
- Default example app with a Service and RxJS instead of the actual hello world.

sdasd
### Environment requirements:
- git
- docker v1.10 or above
- docker-compose v1.6.0 or above

### Docker Preview
- ```docker-compose build```
- ```docker-compose -f environment/development.yaml up -d``` -d starts docker as daemon
- ```docker-compose -f environment/development.yaml logs -f``` to monitor docker output

### Dry NPM Preview
- ```npm i```
- ```npm run watch```
- ```visit: http://localhost:8180```

### Tasks

- ```npm run lint``` - lint js/ts.
  - ```npm run jshint``` - javascript linter.
  - ```npm run tslint``` - typescript linter.
  - ```npm run jscs``` - javascript code style.
- ```npm run clean``` - npm folder/cache, dist, reports folders.
  - ```npm run clean:dist``` - clean dist folder.
- ```npm run build:dev``` - clean dist + dev build.
- ```npm run build:prod``` - clean dist + prod build.
- ```npm run watch``` - dev build + watch + run server on dev port.

### Spin up production environment
- ```docker-compose build```
- ```docker-compose -f environment/production.yaml up -d```
