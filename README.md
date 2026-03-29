# @xhuliom/capacitor-apple-sign-in

Capacitor 8 compatible fork of [`@capacitor-community/apple-sign-in`](https://github.com/capacitor-community/apple-sign-in).

> **Fork note:** This is a fork of the original [capacitor-community/apple-sign-in](https://github.com/capacitor-community/apple-sign-in) plugin by the Capacitor Community contributors. The only change is updating the Swift Package Manager dependency from `capacitor-swift-pm` 7.x to 8.x for Capacitor 8 compatibility. All credit for the original implementation goes to the original authors. Licensed under MIT.

## Installation

- `npm i @xhuliom/capacitor-apple-sign-in`
- `npx cap update`

## Usage (iOS, Web)

```ts
import {
  SignInWithApple,
  SignInWithAppleResponse,
  SignInWithAppleOptions,
} from '@xhuliom/capacitor-apple-sign-in';

const options: SignInWithAppleOptions = {
  clientId: 'com.your.webservice',
  redirectURI: 'https://www.yourfrontend.com/login',
  scopes: 'email name',
  state: '12345',
  nonce: 'nonce',
};

SignInWithApple.authorize(options)
  .then((result: SignInWithAppleResponse) => {
    // Handle user information
    // Validate token with server and create new session
  })
  .catch(error => {
    // Handle error
  });
```

###

## Instructions (Android)

Not supported.
