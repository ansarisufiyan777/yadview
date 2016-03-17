**yadview** is a fork of the AOSP DayView. It loads, lays out and displays events.  yadview is intended to be more robust in handling of events from various sources, rendering differently.


# Getting Started #
yadview can be integrated into an Activity or Fragment with low effort.  A few easy steps to get started:
  1. Create your view, with a `ViewSwitcher` in place to hold your schedule view
  1. Create a `com.google.code.yadview.EventResource` to supply the events in your schedule
  1. In your Activity/Fragment's `onCreate()`, initialize your `ViewSwitcher` with a `ViewFactory` implementation - you can use a `com.google.code.yadview.impl.DefaultDayViewFactory` to get started


For an example of an activity that is a bit more complex, browse the GIT repository to view.
  * https://code.google.com/p/yadview/source/browse/yadview-harness/src/com/google/gode/yadview_harness/MainActivity.java is a simple starter activity
  * https://code.google.com/p/yadview/source/browse/yadview-harness/src/com/google/gode/yadview_harness/YadviewHarnessDayViewFactory.java is a sample ViewFactory implementation which introduces customizations of how events are displayed.

Sample single-day schedule view, using a custom event renderer:
![https://yadview.googlecode.com/git/com.google.code.yadview/wiki-content/yadview-single-day.png](https://yadview.googlecode.com/git/com.google.code.yadview/wiki-content/yadview-single-day.png)

yadview depends on [Guava](https://code.google.com/p/guava-libraries/).