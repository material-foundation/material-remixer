# material-remixer

Remixer is a set of cross-platform libraries and protocols to allow live adjustment
of apps and prototypes during the development process. It is supported on Android, iOS and Web.

---

## Core concepts

Remixer allows you to add variables that you can tweak and triggers that you can interact with in all of its interfaces. All of those tweaks and interactions will be reflected immediately in the UI.

### Triggers

Triggers are a convenient way to simulate events happening, to rapidly test event handling. They just run a callback when pulled.

### Variables

A variable lets you tweak one value of any of the supported types.

#### Supported data types

Remixer currently supports:
- Boolean
- String
- Numbers (floats on iOS and Web, Integers on android)
- Colors (represented as integers on Android)

#### Variable specializations
* __Item List Variable__: Allows you to choose from a list of possible values (List of colors, for example).
* __Range Variable__: Allows you to choose a numerical value in a specific range (Range of text sizes between 16 and 28, for example).

## Modes of operation

Remixer will offer two modes of operation: local only, where your tweaks, triggers etc are only reflected on your local device; and cloud mode where any interaction with remixer is reflected across all devices and saved/synced to a cloud service.

### Local-only mode
Local only mode saves the variable values across application restarts and allows you to share the current configuration as a JSON file.

### Cloud mode
Cloud mode will be supported by a companion Firebase application (the Web Dashboard), that provides syncing, pushing values and becomes the source of truth for Remixer. In cloud mode, Remixer would reference variables and triggers that are defined and configured in the Web Dashboard.

Cloud mode enables us to build integrations with design tools such as Sketch, and is what we envision will be the future of Remixer.

_Note_: The iOS version of remixer has a proof of concept of this functionality, you can find it in the **cloud_exp** branch in the iOS repository. By virtue of this being a proof of concept, it is expected that there will significant API changes both in the iOS and Web Dashboard sides.

## Repositories

Platform specific libraries and tools can be found in the following GitHub repos:

  - [iOS](https://github.com/material-foundation/material-remixer-ios) - Remixer for iOS.

  - [Android](https://github.com/material-foundation/material-remixer-android) - Remixer for Android.

  - [Web](https://github.com/material-foundation/material-remixer-web) - Remixer for Web.

  - [Dashboard](https://github.com/material-foundation/material-remixer-dashboard) - Remixer web dashboard for all platforms.
