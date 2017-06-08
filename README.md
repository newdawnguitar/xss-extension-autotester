# xss-extension-autotester
Run this to automatically test your 6262 XSS extension against various inputs 

#Setup
1 - Install Node
2 - Clone this repo to your computer
3 - Install dependencies via npm -> npm i

# How to Run
1 - Edit "relativePateOfExtension" variable in test.js to point to the relative path to the folder of your extension
2 - Run via command -> Node test.js

# How it works
This uses Selenium to automate testing. First, it grabs each input from the local file scripts.txt, and checks each one through the provided link to see if it should be passed or not. Once finished, it reloads Selenium, this time with your extension, and checks each input again to see if it has been sucessfully blocked or not.

# Please Contribute
Please add test cases to scripts.txt (each on a new line) and submit a pull request so we can have more to test against.
