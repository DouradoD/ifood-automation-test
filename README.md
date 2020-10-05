# ifood-automation-test
First of all, thanks for being here, we hope you can succed on this test :)
Let's move on with some small rules...

## Business rules
* Develop at least 3 test scenarios validating the most important / relevant uses of the aplication.
* If you find any bugs on the app, add a note on your PR with how to reproduce, and prioritize the severity as you think.
* Feel free to run this on any kind of simulator or device, just let us know how you have run.

### Hints
* Some of our stack on iFood are: Java, Espresso, XCUI and Appium. Oh, we have our own API framework with JavaScript as well.
* Everything we run we use a jenkinsFile on Jenkins.

## Non functional requirements
* Briefly elaborate on your solution,w architecture details, choice of patterns and frameworks.
* Use whatever language, tools and frameworks you feel comfortable to, but keep an eye on the hints section.
* Fork this repository and submit your code.

## App Info
* Login: teste@teste.com
* Password: 123456

# Execute the automated tests
###Note: 
Setup the capabilities to recognize your device/emulator in ...
src/test/java/capabilities/CapsAndroid.java
or 
src/test/java/capabilities/CapsIOS.java

### Android
mvn clean verify -P serenity -Dplatform=android -Dcucumber.options="--tags '@android'"
### iOS
mvn clean verify -P serenity -Dplatform=ios -Dcucumber.options="--tags '@ios'"


##To view the report related to the last execution local in the Diogo Dourado machine
Open the following file using Chrome

Android
```
last-report/android/site/serenity/index.html
```

iOS
```
last-report/ios/site/serenity/index.html
```