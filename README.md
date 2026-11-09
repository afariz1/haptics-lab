# Haptics Lab

Interactive playground for haptic + sound feedback on phones. Companion to the TAMa essay
*Multisensory Feedback (Haptics and Sounds)*, FIT VUT Brno 2026/27.

**Live:** https://afariz1.github.io/haptics-lab/ (open on an Android phone in Chrome for vibration)

| Tab | What you can try |
|---|---|
| Vibration types | 36 patterns: clicks, strength via PWM, multi-taps, ramps, textures, notification and alarm patterns |
| UI tokens | the 23 Android `MultisensoryManager` tokens (Android 17 QPR2) as web approximations, with code for Android, iOS (SwiftUI), Expo and the web |
| Intensity × sharpness | the 2D model shared by Core Haptics and Android envelopes; tap to hear/feel, get code |
| Gestures | detent slider, pull to refresh, long press, swipe to delete, surface textures |
| Keyboard | per-key tokens vs one click vs too strong vs none |
| Combine | any haptic × any sound, matched vs mismatched pairs, ghost haptic |
| Timing | touch-to-feedback delay (blind test), sound vs vibration offset with latency compensation |
| Composer | build patterns from pulses (length, intensity, sharpness) and gaps; export to Web, Android `createWaveform`, iOS AHAP, React Native |
| Rhythm | haptic metronome with accents |
| Device | capabilities, shortest pulse you can feel, motor response test |

Notes: the Web Vibration API only switches the motor on/off, so softer pulses are made with PWM.
iOS Safari has no vibration API; the page plays sound and shows the pattern, plus an optional
experimental single-tap via Safari's switch control. Single HTML file, no dependencies.
