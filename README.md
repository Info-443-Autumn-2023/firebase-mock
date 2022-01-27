# Firebase Mock (Wi 22)

This repository contains code for (partially) mocking Firebase in Jest. Mocks v9 of the Firebase SDK only.

Current functionality:
- Authentication: `onAuthStateChange` is stubbed and will automatically "log in" a mock user
- Realtime Database: mocks most methods, including `set`, `push` and `onValue`. Promise-based methods will not produce errors errors.

## Usage
Copy the `setupTests.js` file into the `src` folder of a Create React App project. This will mock or stub No further configuration should be necessary.

## Customization 
You can customize the "initial" realtime database contents or the details about the mock authenticate user by modifying the `MOCK_INITIAL_DATA` and `MOCK_USER` constants.