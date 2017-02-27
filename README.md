![remixer](https://cdn.rawgit.com/material-foundation/material-remixer/master/docs/assets/lockup_remixer_icon_horizontal_dark_small.svg)

Remixer helps teams use and refine design specs by providing an abstraction for these values that is accessible and configurable from both inside and outside the app itself. This abstraction is called a variable. A variable has a key (e.g. "primaryColor"), a type (e.g. Color), and a value (e.g. red). Instead of hard-coding values, engineers can use variables to allow anyone on their team to refine them during development without even having to restart the app. Refinements can be done from inside the app itself, from a web remote controller, or through plugins for other design tools.

The Remixer SDK is currently under development and will be available for iOS, Android and Web. Please review the State of Development table for status of each platform.

## Variables

A Remixer variable has a unique key associated with it, and supports the following data types:


- **Numbers** 
	- Example: Use a numeric variable to define how long an animation should run for.
	- If you want to limit a numeric variable to be inside a certain range you can use a Range variable. A range variable can also be configured to be continuous or discrete (fixed increment value).

- **Colors**
	- Example: Use a color variable to reference a code in your color palette instead of hardcoding its value. This way there’s no need to update every instance of the old color in your codebase when the palette changes.

- **Booleans**
	- Example: Use a boolean variable to hide or show a view during development.

- **Strings**
	- Example: Use a string variable to easily try different options for a header.

Remixer also supports setting a list of values a variable can be set to. For example, a color variable can be configured so that its value can only be changed to red, blue or yellow.

## Web Remote Controller

If enabled, the variables defined in your app will be exposed on a remote controller website. Share the link to this site with your teammates from within the overlay or by emailing them. The remote controller allows updating the defined variables, and changes will be propagated in real-time across associated apps.

## Roadmap and State of development

Development of Remixer is ongoing across the supported platforms. Visit our [State of Development](https://github.com/material-foundation/material-remixer/wiki/State-of-Development) wiki which details the status of development for each platform. In addition, visit our current [Roadmap](https://github.com/material-foundation/material-remixer/wiki/Roadmap) wiki for a list of features planned for future releases.

## Repositories

Platform specific libraries and tools can be found in the following GitHub repos:

- [iOS](https://github.com/material-foundation/material-remixer-ios) - Remixer for iOS.
- [Android](https://github.com/material-foundation/material-remixer-android) - Remixer for Android.
- [JavaScript](https://github.com/material-foundation/material-remixer-js) - Remixer for JavaScript.
- [Web Remote](https://github.com/material-foundation/material-remixer-remote-web) - Remixer web remote controller for all platforms.

## Is Material Foundation affiliated with Google?

Yes, the [material-foundation](https://github.com/material-foundation) organization is one of Google's new homes for tools and frameworks related to our [Material Design](https://material.io) system. Please check out our blog post [Design is Never Done](https://design.google.com/articles/design-is-never-done/) for more information regarding Material Design and how Remixer integrates with the system.

## Contributing

We gladly welcome contributions! If you have found a bug, have questions, or wish to contribute, please follow our [Contributing Guidelines](https://github.com/material-foundation/material-remixer/blob/master/CONTRIBUTING.md).

## License

© Google, 2016. Licensed under an [Apache-2](https://github.com/material-foundation/material-remixer/blob/master/LICENSE) license.
