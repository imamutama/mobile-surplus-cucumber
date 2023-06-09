
## Prerequisites
* Java JDK 11 or higher installed
* Maven installed
* Android real device (or emulator) connected and accessible
* Install Appium
* Setup environment variable SDK

## Setup
Clone the repository: 
```console
git clone https://github.com/imamutama/mobile-surplus-cucumber.git
```
* Start Appium Driver

## Configuration
Open the android-real-devices.json file in the project's capabilities-json/android-real-device.json resources directory.
Set the value of json:

```console
{
  "platformName": "Android",
  "deviceName": "oreo",
  "platformVersion": "12.0",
  "appPackage": "com.loginmodule.learning",
  "appActivity": "com.loginmodule.learning.activities.LoginActivity",
  "udid": "9T9PMZEYO7MR9DJB",
  "newCommandTimeout": 10,
  "noReset": false
}
```
## Running Tests
To run the automation tests, use the following command:
```console
$ mvn clean test -Dcucumber.filter.tags="@smoke-test" -Denv.PLATAFORM=ANDROID_REAL_DEVICE
```
This command will execute the tests tagged with @smoke-test on an Android real device.

## Test Scenarios
The project includes various test scenarios covering different aspects of Salesforce UI. Some of the key test scenarios are:

* Login
* Registration

