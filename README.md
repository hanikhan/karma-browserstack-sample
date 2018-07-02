 Karma-BrowserStack Example for iOS with bs-local.com
=========

Sample for using karma-browserstack-launcher to run Karma tests (QUnit framework) on BrowserStack infrastructure.
One test is failing on purpose as a demo of BrowserStack catching bugs in different browsers.

### Prerequisites
Node and npm

### Clone this repository
`git clone https://github.com/hanikhan/karma-browserstack-sample.git`

### Install dependencies

Navigate to appropriate directory for testing and then install the dependencies by running

`npm install`

### BrowserStack Configuration

Export the environment variables for the username and access key of your BrowserStack account.
These can be found on the automate dashboard page on [BrowserStack](https://automate.browserstack.com/).

`export BROWSERSTACK_USERNAME=<browserstack-username>`

`export BROWSERSTACK_KEY=<browserstack-access-key>`

You can further customize configuration in karma.conf.js. For detailed reference, visit karma-browserstack-launcher github repository [here](https://github.com/browserstack/karma-browserstack-launcher).

When running the tests using Travis, set the username and key under Travis from:
More Options > Settings > Environment Variables

`BROWSERSTACK_USERNAME=<browserstack-username>`

`BROWSERSTACK_KEY=<browserstack-access-key>`

#### Run the tests

Execute the following command to run the karma tests:

`npm test`
