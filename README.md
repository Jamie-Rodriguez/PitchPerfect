# Pitch Perfect
This is my version of the Pitch Perfect iOS app that is built during the Udacity course [Intro to iOS App Development with Swift](https://www.udacity.com/course/intro-to-ios-app-development-with-swift--ud585).

I thought I would post my solution as I completed the course in January 2018 and did notice some outdated features to Xcode and iOS that have become deprecated since the course was written which may be confusing to a beginner.

## Issues
### *Top/Bottom layout guide* has been deprecated by the *Safe Area* construct
This is encountered in *Lesson 5: Playback and Audio Effects - 6. StackViews for Echo+Reverb and Stopping Playback*.

The *Top/Bottom layout guide* has been deprecated since iOS 11.0, and replaced with the *Safe Area* construct.

In order to recreate the layout, the *Safe Area* should be referenced instead of *Top/Bottom layout guide*.

### Possible bug with *content mode* not applying to button images
*Lesson 5: Playback and Audio Effects - 7. Fixing the UI* mentions that changing the buttons' *content mode* to *Scale Aspect Fit* is key to fixing the stretching of the button images on smaller devices. However simply changing the *content mode* of a button in the *Attributes Inspector* did not fix the behaviour.

Instead, I was able to reach a solution by setting the *content mode* in the *viewDidLoad* function.
