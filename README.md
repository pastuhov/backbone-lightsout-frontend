## Getting started ##

You will need to download and install [Node](http://nodejs.org/) to fetch the
dependencies and use the build tools.

## Updating dependencies ##

Third party packages may update independently from this main repo, so it's a
good idea to update after fetching.

``` bash
npm install
```

## Build process ##

The build process consists of numerous Grunt plugin tasks that work together
to optimize your application.

``` bash
# To run the build process, run the NPM start script. This will automatically
# run JSHint, the development Connect server, and watch your files for changes.
npm start

# Run a build and test the now optimized assets.
npm run test-prod
```

## Working with tests ##

Ceate an ES6 module in the `test/tests` directory and add an
import in the `test/runner.js` file. You'll see existing examples in there to
make it easy to follow.

Run the tests with:

``` bash
npm test
```

If you want to continuously test, run `npm start` and open the
`test/index.html` file in your browser. The tests will re-run whenever you
change source files.

By default, the test runner is BDD Mocha and uses Node's assert.
