# Sendbird React UIKit Sample Application Walkthrough with Automation Testing and CI Integration
Task for automation testing using Selenium Java and CI Integration

## To use the framework:

1. Fork this repository.
2. Clone, i.e, download your copy of the repository to your local machine using
```
git clone https://github.com/[your_username]/selenium-java-test-automation-architecture.git
```
3. Import the project in IntelliJ IDEA.
4. Make your changes.
5. Run the test.

## The project uses the following:

- *[Java 21]([https://openjdk.java.net/projects/jdk/11/](https://openjdk.org/projects/jdk/21/))* as the programming language.
- *[Selenium WebDriver](https://www.selenium.dev/)* as the web browser automation framework using the Java binding.
- *[TestNG](https://testng.org/doc/)* as the testing framework.
- *[IntelliJ IDEA](https://www.jetbrains.com/idea/)* as the IDE.

## Basic Usage

- ### Configuration
  The projects set some static data, like appId, if you want to change the static data, just change it on the Java file. Some dynamic data will be generated by the code like userId and nickname.
  
- ### Browser
  The project contains the implementation of the *Chrome* browser.

- ### Tests
  The project uses *TestNG* as the test runner. Check [this implementation](./src/test/java/io/github/tahanima/e2e/LoginTest.java) for reference.

  #### Code Steps
  1. Open a new driver (Chrome)
  2. Go to URL https://sendbird-uikit-react.netlify.app/url-builder
  3. Fill in data for userId 1 and copy the URL
  4. Open chat room for userId 1
  6. Fill in data for userId 2 and copy the URL
  7. Open chat room for userId 2
  8. Back to chat room of userId 1
  9. Send 3 messages (Text, Image and file txt)
  10. Verify messages on chat room of userId 2
  11. Close driver
