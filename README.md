# Thanx_take_home_proj

ANDROID BUILD on Windows machine: 


DEPENDENCIES:

	Ensure the following dependecies are already set up: 
	 - node             			https://nodejs.org/en/download/ 
	 - ruby             			https://www.ruby-lang.org/en/documentation/installation/ 
	 - java and jdk 8 (must be 8 not 15)  	https://java.com/en/download/manual.jsp 
			    			https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html
	 - gradle           			https://gradle.org/install/ 
	 - react native     			https://reactnative.dev/ 
	                    			https://github.com/expo/create-react-native-app 
	 - android studio (android sdk): 	https://developer.android.com/studio 

	Ensure environment variables and paths are configured for each depenency above 
	(ie: JAVA_HOME, ANDROID_HOME etc)

	in android sdk (%ANDROID_HOME%\tools\bin)
	run "sdkmanager --licenses" and agree to all the licenses

	PACKAGES:
		in the command terminal...
		run "npm install" to ensure all the correct packages are loaded onto the system 
		run "gem install fastlane" to install dependecies for fastlane 


BUILDING LOCALLY WITH FASTLANE:

	in the command terminal run "fastlane android build"

	successfull build should give a summary like this:
	+------+----------------------------+-------------+
	|                fastlane summary                 |
	+------+----------------------------+-------------+
	| Step | Action                     | Time (in s) |
	+------+----------------------------+-------------+
	| 1    | Verifying fastlane version | 0           |
	| 2    | ensure_git_branch          | 0           |
	| 3    | ensure_git_status_clean    | 0           |
	| 4    | git_pull                   | 1           |
	| 5    | clean                      | 45          |
	| 6    | assembleDebug              | 101         |
	+------+----------------------------+-------------+

	[20:52:36]: fastlane.tools finished successfully 🎉


TRAVISCI:
https://travis-ci.com/github/brichi15/thanx_take_home/builds

pushing to master branch will trigger a build in travisCI


