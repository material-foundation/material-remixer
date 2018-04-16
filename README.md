# DEPRECATED

Remixer is no longer in active development.  It was an experiment by the Material Design team at Google, which we may return to some day, but at this time we have no plans to continue development here.

For more information about the projects we're actively working on, please visit:

[material.io](https://material.io/)

---

Remixer allows you to easily define UI variables in your app that can be adjusted while it is running. This can help you and your team to iterate very quickly on design issues because you don't need to rebuild or even restart your app to see the changes reflected.

Remixer is available in three platforms ([Android](http://github.com/material-foundation/material-remixer-android), [iOS](http://github.com/material-foundation/material-remixer-ios) and [JavaScript](http://github.com/material-foundation/material-remixer-js)) and all of them support setting up a [Remote Controller](http://github.com/material-foundation/material-remixer-remote-web) that lets you change variables from a web dashboard.

| Project | Continuous Integration | Code Coverage | Release |
|---------|------------------------|---------------|---------|
| [Android](http://github.com/material-foundation/material-remixer-android) | [![TravisCI Build Status](https://travis-ci.org/material-foundation/material-remixer-android.svg?branch=develop)](https://travis-ci.org/material-foundation/material-remixer-android) [![CircleCI Build Status](https://circleci.com/gh/material-foundation/material-remixer-android.svg?style=shield)](https://circleci.com/gh/material-foundation/material-remixer-android) | [![codecov](https://codecov.io/gh/material-foundation/material-remixer-android/branch/develop/graph/badge.svg)](https://codecov.io/gh/material-foundation/material-remixer-android) | [![Release](https://jitpack.io/v/material-foundation/material-remixer-android.svg )](https://jitpack.io/#material-foundation/material-remixer-android) |
| [iOS](http://github.com/material-foundation/material-remixer-ios) | [![Build Status](https://travis-ci.org/material-foundation/material-remixer-ios.svg?branch=develop)](https://travis-ci.org/material-foundation/material-remixer-ios) | [![codecov](https://codecov.io/gh/material-foundation/material-remixer-ios/branch/develop/graph/badge.svg)](https://codecov.io/gh/material-foundation/material-remixer-ios) | [![CocoaPods](https://img.shields.io/cocoapods/v/Remixer.svg)]() |
| [JavaScript](http://github.com/material-foundation/material-remixer-js) | [![Build Status](https://travis-ci.org/material-foundation/material-remixer-js.svg?branch=develop)](https://travis-ci.org/material-foundation/material-remixer-js) | [![codecov](https://codecov.io/gh/material-foundation/material-remixer-js/branch/develop/graph/badge.svg)](https://codecov.io/gh/material-foundation/material-remixer-js) | [![npm version](https://badge.fury.io/js/material-remixer.svg)](https://badge.fury.io/js/material-remixer) |
| [Remote Controller](http://github.com/material-foundation/material-remixer-remote-web) | [![Build Status](https://travis-ci.org/material-foundation/material-remixer-remote-web.svg?branch=develop)](https://travis-ci.org/material-foundation/material-remixer-remote-web) |  | [![npm version](https://badge.fury.io/js/material-remixer-remote-web.svg)](https://badge.fury.io/js/material-remixer-remote-web) |

## Variables

A Remixer variable has a unique key associated with it, and can be of type Boolean, Color, Number or String.

Variables support being constrained to a limited set of values to give you better control of what can change. Numeric variables can also be configured as continuous or discrete ranges.

## Web Remote Controller

Remixer can be configured to use a [Remote Controller](http://github.com/material-foundation/material-remixer-remote-web). In this mode your variables can be changed from outside the app, allowing you to collaborate with other people and keep your UI free of overlays. Make sure to check out the [Remote Controller repo](http://github.com/material-foundation/material-remixer-remote-web) to learn more about this feature.

For details on how to set up this mode in your app, please visit one of the platform specific repos.

## Is Material Foundation affiliated with Google?

Yes, the [material-foundation](https://github.com/material-foundation) organization is one of Google's new homes for tools and frameworks related to our [Material Design](https://material.io) system. Please check out our blog post [Design is Never Done](https://design.google.com/articles/design-is-never-done/) for more information regarding Material Design and how Remixer integrates with the system.

## Contributing

We gladly welcome contributions! If you have found a bug, have questions, or wish to contribute, please follow our [Contributing Guidelines](https://github.com/material-foundation/material-remixer/blob/master/CONTRIBUTING.md).

## License

© Google, 2016. Licensed under an [Apache-2](https://github.com/material-foundation/material-remixer/blob/master/LICENSE) license.
