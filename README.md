## [Hacker's Keyboard](https://play.google.com/store/apps/details?id=org.pocketworkstation.pckeyboard) with Zhuyin Hint Text Layout

This fork of [Klaus's Hacker's Keyboard](https://github.com/klausw/hackerskeyboard) adds a new layout:
- 繁體中文 (台灣；注音對應英文) (zh-TW)

### Improvements
- Updated `build.gradle` and build files for compatibility with newer Android Studio versions (requires manually switching to JDK 11 for successful compilation)
- Added zh-TW language layout with Zhuyin as *AltChars* for keyboard hints
- Included common full-width symbols used in Chinese environments
- Enhanced Hint Characters filter logic to display non-ASCII characters, ensuring Zhuyin symbols appear properly

### Recommended Zhuyin Layout Options
- For larger tablet screens: Use the `full 5-row layout` for optimal Zhuyin typing experience
  ![full-layout](full1.png)
- For smaller screens: The `5-row compat layout` works well, with the quote symbol key (') including semi-colon key (ㄤ) and dash key (ㄦ) as alt-characters, allowing complete Zhuyin typing
  ![compat-layout-1](compat2.png)
  ![compat-layout-2](compat3.png)

### Build Instructions
- Clone this project and open in Android Studio
- Configure Gradle settings to use an older JDK version (recommended: Eclipse Temurin JDK 11.0.26)
- The project uses Gradle Plugin version 7.4.1 and Gradle Wrapper version 8.5
- 