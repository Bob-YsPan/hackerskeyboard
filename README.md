## [Hacker's Keyboard](https://play.google.com/store/apps/details?id=org.pocketworkstation.pckeyboard) with array language layouts

This fork of Hacker's Keyboard adds 2 extra languages:

- APL (named `English (APL) [en_AL]`)
- BQN (named `English (BQN) [en_BQ]`)

They support both the full 5-row layout and the 5-row compact layout.

Suggested options:

- "portrait mode": 5-row compact layout (ignore the "US QWERTY only!" warning, unless you need other layouts); note that some some APL/BQN characters aren't available in the base compact layout - you'll need to configure a gesture for toggling the extension row
- "landscape mode": full 5-row layout
- Lower keyboard height to what you feel is comfortable
- "Theme and label settings → Labelled alternative keys": Show all hint labels
- "Theme and label settings → Keyboard Theme" can be chosen to your liking
- "Auto-capitalisation": off
- "Gesture and key actions": "Toggle extension row" somewhere (note that for the gesture to register, both the start & end point of the touch must be within the keyboard)
- "Ctrl-A (select all) override": "Use Ctrl-A (no override)" to have ctrl+a for Select All
- "Popup mini-keyboard contents" → "Add shifter"
- "Long-press duration": set this to the lowest number you're comfortable with (I've set it to 160ms)
- "Suggested punctuation" → `{}[]()` (as those are harder to type in compact portrait otherwise)

Build APK: `./gradlew assembleRelease` with java 11 (8 maybe works, haven't tested); output is at `app/build/outputs/apk/release/app-release.apk`