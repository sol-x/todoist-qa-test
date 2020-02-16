# Todoist test

Please create the three automation tests for the [Todoist](https://todoist.com/?lang=en) Android application and API that are specified below.

The [Todoist Android app can be downloaded here](https://www.apkmirror.com/apk/doist/todoist/todoist-15-0-4-release/todoist-to-do-list-tasks-reminders-15-0-4-android-apk-download/) or using the Play store from within the Android emulator.

## Instructions
 - Please approach your code architecture as if this will be the beginning of a large QA project.
 - Create a Todoist test user manually using email (not google or facebook). Please bear in mind that your test code will include your account key so do not use your own personal Todoist account if you already have one.
 - Use an Android emulator for tests, e.g. [Genymotion](https://www.genymotion.com/) or [Android studio](https://developer.android.com/studio).
 - Tests should include multiple assertions where appropriate.
 - For Automation Framework you can use [appium](http://appium.io/) or similar.
   - The tests should be written in code (Java, Python, JavaScript etc.) not created via postman or similar.
   - You can use whatever REST client you need for interacting with the API, e.g. [axios](https://github.com/axios/axios) for JavaScript.

## Tests to implement

Note that all steps should be performed in the mobile app, except where you see the text *using the API*. You can find instructions about how to use the [Todoist API here](https://developer.todoist.com/rest/v1/).

### Test 1, project creation via the Todoist API
 - Create a project named "API test project" using the Todoist API.
 - Login into mobile application.
 - Verify that mobile app can see the project.

### Test 2, task creation via the Android app
 - Create project named `Android test project` using the Android app.
 - Create task task named `Android test task` inside of the `test` project.
 - Verify that `Android test task` was created inside of `Android test project` *using the API*.

### Test 3, task creation using the Android app and reopening using the API
 - Open mobile application
 - Create test project named `second test project`.
 - Add a task named `second test task` to `second test project`.
 - Set `second test task` as completed.
 - Reopen `second test task` *using the API*.
 - Verify that `second test task` is open in `second test project` *using the android app*.

## Submitting your solution

Please zip/tar the entire test directory and email your solution back to us. Please do not fork the project on git or submit a pull request with your solution as we wish your solution to remain private.

We would like it if you would submit your solution as multiple git commits with descriptive commit messages.
