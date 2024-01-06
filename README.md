# Sample tests for a mobile app

:hammer_and_wrench: One of my **manual testing** practice projects involved testing a simple mobile app, which has recently been published on Google Play Store: [ISTQB Mock Tests](https://play.google.com/store/apps/details?id=com.householdspirits.istqbmocktests4.x0&hl=pl&gl=US).

## The app

* It is a simple, single-user app with two mock ISTQB tests to be taken offline.
* It does not involve creating an account and does not collect any user information.
* It does not allow to enter or edit any input, modify its content, or upload anything.

## Test suite

:scroll: The test suite in this repo contains an overview of all **test scenarios and test cases** for testing the app on an Android emulator (see section below). As for detailed test cases, I included only a third of them in the file, as it is for presentation purposes only.

:thinking: The biggest challenge was to determine the **level of detail** of test scenarios and corresponding test cases. Another difficulty was to generate **negative test cases**, as the app is rather simple (no input, modification or upload allowed), which made it difficult to trigger unexpected behaviors.

**Responsiveness** was tested on over twenty different screen resolutions. I inluded only two sample resolutions in the test suite attached.

## Test environment

The test suite was executed on an **Android emulator**: LDPlayer v9.0.62(9). After all emulator tests were passed, another set of tests was performed on two **physical devices** - with Android 9 and Android 11. 

:iphone: The test suite for physical devices was almost the same, the only differences being:
* additional test cases for verifying correct installation on devices;
* an additional test case for navigating between test questions by swiping the touch screen (see scenario TS-08);
* no test cases for various screen resolutions (see scenario TS-25). 