# xss-extension-autotester
Run this to automatically test your 6262 XSS extension against various inputs.
### Installation
This requires [Node.js](https://nodejs.org/) to run.

Clone the repo and install the dependencies.

```sh
$ cd xss-extension-autotester
$ npm i
```

### Running

Use the commands below to run. Make sure you define the relative path of the location of the extension!

```sh
$ cd xss-extension-autotester
$ Node test.js -e /path/to/extension/folder
```

### What's going on here?
This uses Selenium to automate testing. First, it grabs each input from the local file scripts.txt, and checks each one through the provided link to see if it should be passed or not. Once finished, it reloads Selenium, this time with your extension, and checks each input again to see if it has been sucessfully blocked or not.

### Please Contribute Tests
Let's help eachother with some tests! Please add test cases to scripts.txt (each on a new line) and submit a pull request so we can have more to test against.

### Compatibility
I have only tested this on Mac OSX. Works on that platform.
