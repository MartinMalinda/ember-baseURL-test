# Base-url

|                              | Ember CLI 2.6 - manually added `<base>`                                                                                                           | Ember CLI 2.6 - autopopulated `<base>`                                                                     | Ember CLI 2.7 - no `<base>` | Ember CLI 2.7 - manually added `<base>`                                                                                                            |
|------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|---------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| baseURL set, rootURL set     | `Uncaught Error: Assertion Failed: Path /base-test does not start with the provided rootURL /root-test/`                                        | `Uncaught Error: Assertion Failed: Path /base-test does not start with the provided rootURL /root-test/` | 404, can't find assets    | `Uncaught Error: Assertion Failed: Path /base-test does not start with the provided rootURL /root-test/`                                         |
| baseURL set, rootURL unset   | OK / two `<base>` tags                                                                                                                            | OK                                                                                                       | OK                        | OK / two `<base>` tags                                                                                                                             |
| baseURL unset, rootURL set   | error after hard refresh: `Uncaught Error: Assertion Failed: Path /manual-test/root-test/ does not start with the provided rootURL /root-test/` | 404, can't find assets                                                                                   | OK                        | error after hard refresh:  `Uncaught Error: Assertion Failed: Path /manual-test/root-test/ does not start with the provided rootURL /root-test/` |
| baseURL unset, rootURL unset | OK                                                                                                                                              | OK                                                                                                       | OK                        | OK                                                                                                                                               |

This README outlines the details of collaborating on this Ember application.
A short introduction of this app could easily go here.

## Prerequisites

You will need the following things properly installed on your computer.

* [Git](http://git-scm.com/)
* [Node.js](http://nodejs.org/) (with NPM)
* [Bower](http://bower.io/)
* [Ember CLI](http://www.ember-cli.com/)
* [PhantomJS](http://phantomjs.org/)

## Installation

* `git clone <repository-url>` this repository
* change into the new directory
* `npm install`
* `bower install`

## Running / Development

* `ember server`
* Visit your app at [http://localhost:4200](http://localhost:4200).

### Code Generators

Make use of the many generators for code, try `ember help generate` for more details

### Running Tests

* `ember test`
* `ember test --server`

### Building

* `ember build` (development)
* `ember build --environment production` (production)

### Deploying

Specify what it takes to deploy your app.

## Further Reading / Useful Links

* [ember.js](http://emberjs.com/)
* [ember-cli](http://www.ember-cli.com/)
* Development Browser Extensions
  * [ember inspector for chrome](https://chrome.google.com/webstore/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi)
  * [ember inspector for firefox](https://addons.mozilla.org/en-US/firefox/addon/ember-inspector/)

