# flylm32 Unity asset recovery — iOS investigation

This archive contains original Unity game data recovered from the Android APK, not a functioning Unity Editor project or iOS IPA.

## Contents
- `recovered/`: preserved original Unity data paths (scenes, serialized assets, resources, metadata where available).
- `manifest.json`: source hash and extracted-file inventory.

## What remains necessary
1. Obtain the original Unity project (preferred), or inspect and manually reconstruct compatible scenes, scripts and assets using authorized Unity asset tooling.
2. Restore game logic: Android IL2CPP binaries cannot run on iOS, and recovered metadata alone is not C# source.
3. Replace Android-only plugins and APIs with iOS equivalents.
4. Use Unity with iOS Build Support and Xcode on macOS to build, sign and export an IPA.

This package alone cannot be installed on iPhone. No claim is made that a faithful reconstruction is possible.
