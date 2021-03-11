6DoF for the Cardboard SDK!
====================================
This is a fork of the [Google Cardboard XR Plugin for Unity](https://github.com/googlevr/cardboard-xr-plugin/) to support 6DoF (roomscale) tracking. Instead of being fixed in place you can walk around!

This uses a modified version of the Cardboard SDK [found here](https://github.com/Aryzon/cardboard/)

We made this to support the [Aryzon MR headsets](https://aryzon.com) however all other VR Cardboard headsets are supported with one condition, the camera must be able to see the world. Furthermore your phone must be able to run ARCore or ARKit.

We use **ARFoundation** to feed 6DoF data to the Cardboard SDK. This means you can use all the goodies from [ARFoundation](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@4.1/manual/index.html) like plane detection etc!


## Get started

The Quickstart link below shows the default settings for Cardboard without 6DoF.
Follow the instructions however apply these changes:

1) Replace the package link with this: https://github.com/Aryzon/cardboard-xr-plugin.git
2) In the package manager add ARFoundation and ARCore for Android or ARKit for iOS. The sample scene is made with version 2.1.6 but I suggest to try the highest stable version. We tested it up to 4.1.5 (you may need to change enum values on the ARCameraManager).
3) Do **NOT** enable the Cardboard XR Plugin in XR Plug-in Management. Instead enable ARCore and/or ARKit.
4) Add CARDBOARD_6DOF to the scripting define symbols (found in 'Player Settings' -> 'Other').
5) From the sample scenes use 6DoF

To get started with the Google Cardboard XR Plugin for Unity, see:

* [Quickstart for Unity](//developers.google.com/cardboard/develop/unity/quickstart)


## API reference

* [Google Cardboard XR Plugin for Unity API Reference](//developers.google.com/cardboard/reference/unity)


## Release notes

The SDK release notes are available on the
[releases](//github.com/googlevr/cardboard-xr-plugin/releases) page.


## Roadmap

The project roadmap is available on the
[Projects](https://github.com/googlevr/cardboard/projects/1) page.


## Contributing

Please read and follow the steps in [CONTRIBUTING.md](/CONTRIBUTING.md) file.


## License

Please see the [LICENSE.md](/LICENSE.md) file.


## Brand guidelines

The "Google Cardboard" name is a trademark owned by Google and is not included
within the assets licensed under the Apache License 2.0. Cardboard is a free
and open-source SDK that developers can use to create apps that are compatible
with the Google Cardboard VR platform. At the same time, it's important to make
sure that people don't use the "Google Cardboard" mark in ways that could
create confusion.

The guidelines below are designed to clarify the permitted uses of the "Google
Cardboard" mark.

**Things you can do**:

* Use the "Google Cardboard" mark to describe or refer to apps developed with
  the Cardboard SDK in ways that would be considered "fair use."
* Use the "Google Cardboard" mark to make truthful factual statements regarding
  the compatibility or interoperability of your app. For example, "This app is
  compatible with Google Cardboard" or "This app works with Google Cardboard."

**Things you can't do**:

* Don't use the "Google Cardboard" mark in a manner that implies that Google has
  endorsed or authorized your app or that makes your app appear to be an
  official Google product. For example, you shouldn't reference your product as
  "an official Google Cardboard app."
* Don't incorporate the "Google Cardboard" mark into your own product names,
  service names, trademarks, logos, or company names.
* Don't display the "Google Cardboard" mark in a manner that is misleading,
  unfair, defamatory, infringing, libelous, disparaging, obscene or otherwise
  objectionable to Google.
* Don't alter or distort the "Google Cardboard" mark. This includes modifying
  the mark through hyphenation, combination or abbreviation. For example, don't
  say "G Cardboard" or "Google-Cardboard."

In addition to these guidelines, please ensure that you follow the trademark
usage guidelines available here:
https://www.google.com/permissions/logos-trademarks/.
