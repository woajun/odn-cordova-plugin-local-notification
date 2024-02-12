# cordova-plugin-local-notification (notorious fork)

This is a fork of a fork (from [Moodle HQ](https://moodle.com/)) by Notorious. What changed? Other than all the fixes by moodle (up until Android 13 it works fine), now it even works for Android 14, using set() instead of setExact()!

# cordova-plugin-local-notification (fork)

This is a fork of `cordova-plugin-local-notification` by [Moodle HQ](https://moodle.com/). If you are looking for the documentation, you can read the original at [katzer/cordova-plugin-local-notifications](https://github.com/katzer/cordova-plugin-local-notifications).

## Modifications from the original

We created this fork because we needed to include the following modifications in [our mobile application](https://github.com/moodlehq/moodleapp):

| PR | Description |
| -- | ----------- |
| [#1781](https://github.com/katzer/cordova-plugin-local-notifications/pull/1781) | Reuse existing messages when using MessagingStyle |
| [#1853](https://github.com/katzer/cordova-plugin-local-notifications/pull/1853) | Use correct authority name |
| - | Support Android X |
| - | Support sender image |
| - | Fix crash with target SDK 31 |
| - | Declare SCHEDULE_EXACT_ALARM permission |
| - | Fix click notifications in Android 12 |

It also includes some commits that are in master and haven't been released.

You can see all the changes here: [0.9.0-beta.3...moodlemobile:v0.9.0-moodle.11](https://github.com/katzer/cordova-plugin-local-notifications/compare/0.9.0-beta.3...moodlemobile:v0.9.0-moodle.11)

## Installation

You can install this package using the [original installation instructions](https://github.com/katzer/cordova-plugin-local-notifications#installation), but installing this package instead:

```sh
cordova plugin add @moodlehq/cordova-plugin-local-notification@0.9.0-moodle.11
```
