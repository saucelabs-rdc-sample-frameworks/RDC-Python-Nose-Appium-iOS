## Note: This repo is no longer maintained.  Please visit https://github.com/saucelabs-rdc-sample-frameworks/RDC-Python-Nose-Appium-iOS for up to date code.

## Python-Nose-Appium-iOS


This code is provided on an "AS-IS” basis without warranty of any kind, either express or implied, including without limitation any implied warranties of condition, uninterrupted use, merchantability, fitness for a particular purpose, or non-infringement. Your tests and testing environments may require you to modify this framework. Issues regarding this framework should be submitted through GitHub. For questions regarding Sauce Labs integration, please see the Sauce Labs documentation at https://wiki.saucelabs.com/. This framework is not maintained by Sauce Labs Support.

### Environment Setup

1. Global Dependencies
    * [Install Python](https://www.python.org/downloads/)
    * Or Install Python with [Homebrew](http://brew.sh/)
    ```
    $ brew install python
    ```
    * Install [pip](https://pip.pypa.io/en/stable/installing/) to install packages

2. Project Dependencies
	* Install packages (Use sudo if necessary)
	```
	$ pip install Appium-Python-Client sauceclient nose==1.1.0
	```
3. Sauce Credentials
    * In the terminal export your Sauce Labs Credentials as environmental variables:
    Note: For python, appium endpoint should use HTTP endpoint, not HTTPS
    ```
    $ export TESTOBJECT_API_KEY=<your project's api key>
    ```
### Running Tests

Tests in Parallel:
	```
	$ nosetests --processes=8 --process-timeout=500
	```

### Advice/Troubleshooting

1.There may be additional latency when using a remote webdriver to run tests on Sauce Labs. Timeouts or Waits may need to be increased.
    * [Selenium tips regarding explicit waits](https://wiki.saucelabs.com/display/DOCS/Best+Practice%3A+Use+Explicit+Waits)

### Resources
##### [Sauce Labs Documentation](https://wiki.saucelabs.com/)

##### [Appium Documentation](http://appium.io/slate/en/master/)

##### [Python Documentation](https://docs.python.org/2.7/)

##### [Nose Documentation](https://nose.readthedocs.org/en/latest/)

##### [Stack Overflow](http://stackoverflow.com/)
* A great resource to search for issues not explicitly covered by documentation.
