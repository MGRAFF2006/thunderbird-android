# Background sync UI verification

Source commit: `8ea853ddf6598a75a152f6df9a4b6fdb59488d54`. Thunderbird Debug 27.0-SNAPSHOT, FOSS debug APK, on an isolated API 36 emulator without mail accounts.

All three choices were selected, the app process was stopped and reopened, and the selected summary and radio choice were verified. The normal screen is 1080×2400 at 420 dpi; the small screen is 840×1680 at 420 dpi (320×640 dp) with system font scale 2.0. Both the option and help text remained visible without clipping.

The app launcher was exercised first; GeneralSettingsActivity was then opened directly under the rooted test emulator to test general settings without adding an account. No mail synchronization or provider-specific Android settings screen was exercised.
