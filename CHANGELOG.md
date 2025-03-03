## [0.2.0] - April 24, 2019

* Slightly breaking change - on iOS, the sensor was used regardless of what was
  passed to useSensor due to a bug. This meant that even with UI rotation disabled,
  rotation events occured.
* Also switched back to using StatusBarOrientation. It isn't actually deprecated, just
  not advised for normal iOS usage. However, it does what I want and is consistent with
  Android - it returns the orientation of the actual window. If you really want to know
  the orientation of the device, use `useSensor`
* Add buttons to explicitly get rotation using sensor or not (UI)

## [0.1.2] - March 4, 2019

* Reduce amount of orientation changes by keeping track of last change.

## [0.1.1] - March 4, 2019

* Fix documentation and re-order changelog.

## [0.1.0] - March 4, 2019

* Integrate PRs updating to AndroidX and implementing useSensor
* Also made a few changes to do with UseSensor so be careful of that
if you're using the NativeDeviceOrientationCommunicator directly; users
who simply use the widget shouldn't notice anything.

## [0.0.4] - January 2, 2019

* Switch to using UIDeviceOrientation on iOS

## [0.0.2] - June 4, 2018

* Fix name of package

## [0.0.1] - June 4, 2018

* Implement Android & iOS native code.
* Implement Flutter code & widget.
* Write simple example.