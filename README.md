## ![remixer](docs/assets/lockup_remixer_icon_horizontal_dark.png)

Remixer helps teams use and refine design specs by providing an abstraction for these values that is accessible and configurable from outside the app itself. This abstraction is called a Variable. A Variable has a key (e.g. "primaryColor"), a type (e.g. Color), and a value (e.g. red). Instead of hard-coding values, engineers can use Variables to allow anyone on their team to refine them during development without even having to restart the app. Refinements can be done from inside the app itself, from a web dashboard or through plugins for tools like Sketch.

The Remixer SDK is available for iOS, Android and Web.

## Variables

A Variable has a unique key associated with it, and supports the following data types:


- **Numbers** 
	- Example: Use a numeric Variable to define how long an animation should run for.
	- If you want to limit a numeric Variable to be inside a certain range you can use a Range Variable. A Range Variable can also be configured to be continuous or discrete (fixed increment value).

- **Colors**
	- Example: Use a color Variable to reference a code in your color palette instead of hardcoding its value. This way there’s no need to update every instance of the old color in your codebase when the palette changes.

- **Booleans**
	- Example: Use a boolean Variable to hide or show a view during development.
- **Strings**
	- Example: Use a string Variable to easily try different options for a header.

- **Lists**
	- Remixer also supports setting a list of values a Variable can be set to. For example, a color Variable can be configured so that its value can only be changed to red, blue or yellow.


## Triggers

The Remixer library also provides a way to create and use Triggers. Triggers are a convenient way to simulate events in your app, to rapidly test event handling. They just run a callback when triggered.


## Modes of operation

Remixer will offer two modes of operation: Cloud and Local.

### Cloud

Cloud mode is the way to go if you want to use Remixer with a team. In this mode, Variables are defined in a web dashboard and referenced in code. Variables are accessible and configurable through multiple tools, and changes are propagated in real-time. Our first implementation will use Firebase, but we expect to offer other options in the future.

### Local

If you just want to use Remixer to prototype something by yourself, and the in-app overlay is all you need for refining values, then Local mode is for you. Variables are defined in code, and remixer will use your device’s local storage to store any refinements you make.

## Going to production

There is no need to do any code changes when you’re shipping your app. Just use Remixer’s export functionality to export all the values to a single file, and Remixer will take care of the rest. Instead of fetching and syncing values, Remixer will just use this file to get the values for each Variable.


## State of development

|                                                                 |   Android        | iOS |     Web     |
|-----------------------------------------------------------------|:----------------:|:---:|:-----------:|
| String tweaking                                                 |      ✅          | ✅  | ✅          |
| Boolean tweaking                                                |      ✅          | ✅  | ✅          |
| Color tweaking                                                  |      ✅          | ✅  | ✅          |
| Number tweaking                                                 | in progress [^1] | ✅  | ✅          |
| Local storage of variable values                                | in progress      | ✅  | ✅          |
| Sync values across devices                                      | ❌               | ✅  | in progress |
| Create variables from web dashboard                             | ❌               | ❌  | ❌          |
| Override configuration of existing variables from web dashboard | ❌               | ❌  | ❌          |
| Integration with design tools (Sketch et al.)                   | ❌               | ❌  | ❌          |


We expect all of these features to be eventually supported on all platforms as these define our vision for what Remixer should be.

Notes: [^1]: Android's SeekBar only supports integers, we're working on finding a solution that lets us use floats or implement our own.


## Repositories

Platform specific libraries and tools can be found in the following GitHub repos:

- [iOS](https://github.com/material-foundation/material-remixer-ios) - Remixer for iOS.
- [Android](https://github.com/material-foundation/material-remixer-android) - Remixer for Android.
- [Web](https://github.com/material-foundation/material-remixer-web) - Remixer for Web.
- Dashboard - Remixer web dashboard for all platforms (avaialble soon).
