![remixer](https://cdn.rawgit.com/material-foundation/material-remixer/master/docs/assets/lockup_remixer_icon_horizontal_dark_small.svg)

Remixer allows you to easily define UI variables in your app that can be adjusted while it is running. This can help you and your team to iterate very quickly on design issues because you don't need to rebuild or even restart your app to see the changes reflected.

Remixer is available in three platforms ([Android](http://github.com/material-foundation/material-remixer-android), [iOS](http://github.com/material-foundation/material-remixer-ios) and [JavaScript](http://github.com/material-foundation/material-remixer-js)) and comes with a helpful [Remote Controller](http://github.com/material-foundation/material-remixer-remote-web) that lets you interact with variables from another device.

| Project | Continuous Integration | Code Coverage | Release |
|---------|------------------------|---------------|---------|
| [Android](http://github.com/material-foundation/material-remixer-android) | [![TravisCI Build Status](https://travis-ci.org/material-foundation/material-remixer-android.svg?branch=develop)](https://travis-ci.org/material-foundation/material-remixer-android) [![CircleCI Build Status](https://circleci.com/gh/material-foundation/material-remixer-android.svg?style=svg)](https://circleci.com/gh/material-foundation/material-remixer-android) | [![codecov](https://codecov.io/gh/material-foundation/material-remixer-android/branch/develop/graph/badge.svg)](https://codecov.io/gh/material-foundation/material-remixer-android) | [![Release](https://jitpack.io/v/material-foundation/material-remixer-android.svg )](https://jitpack.io/#material-foundation/material-remixer-android) |
| [iOS](http://github.com/material-foundation/material-remixer-ios) | [![Build Status](https://travis-ci.org/material-foundation/material-remixer-ios.svg?branch=develop)](https://travis-ci.org/material-foundation/material-remixer-ios) | [![codecov](https://codecov.io/gh/material-foundation/material-remixer-ios/branch/develop/graph/badge.svg)](https://codecov.io/gh/material-foundation/material-remixer-ios) | [![CocoaPods](https://img.shields.io/cocoapods/v/Remixer.svg)]() |
| [JavaScript](http://github.com/material-foundation/material-remixer-js) | [![Build Status](https://travis-ci.org/material-foundation/material-remixer-js.svg?branch=develop)](https://travis-ci.org/material-foundation/material-remixer-js) | [![codecov](https://codecov.io/gh/material-foundation/material-remixer-js/branch/develop/graph/badge.svg)](https://codecov.io/gh/material-foundation/material-remixer-js) | [![npm version](https://badge.fury.io/js/material-remixer.svg)](https://badge.fury.io/js/material-remixer) |
| [Remote Controller](http://github.com/material-foundation/material-remixer-remote-web) | [![Build Status](https://travis-ci.org/material-foundation/material-remixer-remote-web.svg?branch=develop)](https://travis-ci.org/material-foundation/material-remixer-remote-web) |  | [![npm version](https://badge.fury.io/js/material-remixer-remote-web.svg)](https://badge.fury.io/js/material-remixer-remote-web) |

## Variables

A Remixer variable has a unique key associated with it, and can be a Boolean, Color, Number (represented as floats) or String.

Remixer lets you define a range of values (for variables of type Number), or limit values to members of a list you provide. This lets you ensure that values always _make sense_.

## Web Remote Controller

A separate project, the [Remote Controller](http://github.com/material-foundation/material-remixer-remote-web), is provided for those times when by interacting with Remixer you may make it hard to see the UI you're adjusting. The Remote Controller lets you adjust variable values in a separate device so you can properly appreciate all changes.

Since there is a bit of platform specific setup in each case, look at the documentation in your platform's Remixer Repo  and the Remote Controller's for more information.

## Is Material Foundation affiliated with Google?

Yes, the [material-foundation](https://github.com/material-foundation) organization is one of Google's new homes for tools and frameworks related to our [Material Design](https://material.io) system. Please check out our blog post [Design is Never Done](https://design.google.com/articles/design-is-never-done/) for more information regarding Material Design and how Remixer integrates with the system.

## Contributing

We gladly welcome contributions! If you have found a bug, have questions, or wish to contribute, please follow our [Contributing Guidelines](https://github.com/material-foundation/material-remixer/blob/master/CONTRIBUTING.md).

## License

© Google, 2016. Licensed under an [Apache-2](https://github.com/material-foundation/material-remixer/blob/master/LICENSE) license.
