# ScreenReaderFocusableBug

Summary: Screen Reader Focusable does nothing, even following the exact guidance from the Google documentation.

Google documentation (https://developer.android.com/guide/topics/ui/accessibility/principles#content-groups) says to apply `screenReaderFocusable=true` to the ViewGroup which hosts your UI, and then to apply `focusable=false` to children in order for the group to be read out loud when tapped. This does not work.

Pull down this repo and run the app on an emulator or device with Talkback enabled.

Try clicking in the colored areas outside of the text views and the screen reader will not read the whole content.
