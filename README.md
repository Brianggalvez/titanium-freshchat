# Titanium Freshchat SDK

Use the native Freshchat SDK (iOS / Android) in Titanium

## Example

See the [app.js](./example/app.js) for a full-featured example!

## APIs

### `initialize({ appId, appKey, domain })`

Initializes the SDK. The `domain` is optional.

### `signInUser({ firstName, lastName, email })`

Authenticates a user with Freshchat. All values are optional!

### `updateUserProperty(key, value)`

Updates a given user property (`key`) by it's `value`.

### `signOutUser()`

Resets a user in Freshchat

### `trackEvent(eventName, parameters)`

Tracks an event by a given `eventName`. The `parameters` are optional.

### `showConversations()`

Opens the conversation list.

### `registerForPushNotifications(fcmToken)` (Android only)

Registers the given `fcmToken` with Freshchat. On iOS, this is handled internally by
the corresponding `didRegisterForRemoteNotificationsWithDeviceToken:` selector of the
`UIApplicationDelegate`.

## Author

Hans Knöchel

## License

MIT
