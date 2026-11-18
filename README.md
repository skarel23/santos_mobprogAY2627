### Santos Karel ALwina M.
### 2024-1004162
### INF241

### Laboratory 0: Dicussion 
### Setting up Flutter for the first time had a few bumps, like getting the system PATH variables right, fixing missing Android SDK licenses using flutter doctor, and getting the emulator to actually start. I had to look closely at the error messages in the terminal, run flutter doctor android-licenses to accept the missing agreements, and check online guides to make sure all the native Android tools were installed properly. Working through these issues helped me understand how Flutter connects with native tools like Gradle and the Android SDK. To make things easier in the future, I plan to write down my setup steps and keep all my development tools properly updated from the start. 

### Lab Activity 1: Discussion
### To integrate the Image widget into `newsfeed_card.dart` dynamically, I replaced the static `Placeholder()` widget with a conditional ternary expression checking the boolean `hasImage` property (`hasImage == true ? ... : ...`). When `hasImage` is `true`, the widget renders an `Image.network` container to display the post image; when `hasImage` is `false` on text-only posts, it renders a minimal `SizedBox(height: ScreenUtil().setHeight(1))` so no blank image space appears.