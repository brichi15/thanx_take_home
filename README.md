# Thanx_take_home_proj

ANDROID BUILD on Windows machine:

Ensure the following dependecies are already set up: 
 - node             https://nodejs.org/en/download/ 
 - ruby             https://www.ruby-lang.org/en/documentation/installation/ 
 - java and jdk 8 (must be 8 not 15)  https://java.com/en/download/manual.jsp <br />
		    https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html
 - gradle           https://gradle.org/install/ 
 - react native     https://reactnative.dev/ <br />
                    https://github.com/expo/create-react-native-app 
 - android studio (android sdk): https://developer.android.com/studio

Ensure environment variables and paths are configured for each depenency above 
(ie: JAVA_HOME, ANDROID_HOME etc)


run "npm install" to ensure all the correct packages are loaded onto the system <br />
run "gem install fastlane" to install dependecies for fastlane <br />

FOR BUILDING LOCALLY WITH FASTLANE:
run "fastlane android build"

successfull build should give a summary like this:	<br />
+------+----------------------------+-------------+	<br />
|                fastlane summary                 |	<br />
+------+----------------------------+-------------+	<br />
| Step | Action                     | Time (in s) |	<br />
+------+----------------------------+-------------+	<br />
| 1    | Verifying fastlane version | 0           |	<br />
| 2    | ensure_git_branch          | 0           |	<br />
| 3    | ensure_git_status_clean    | 0           |	<br />
| 4    | git_pull                   | 1           |	<br />
| 5    | clean                      | 45          |	<br />
| 6    | assembleDebug              | 101         |	<br />
+------+----------------------------+-------------+	<br />

[20:52:36]: fastlane.tools finished successfully 🎉



