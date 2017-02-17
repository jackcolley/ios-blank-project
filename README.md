# Blank iOS Project
Blank project for iOS to get up and running FAST. 

# Create iOS project from this blank project:

(below, replace all instances of `coolNewApp` with the name of your new project.)
* `cp -R blank-project/ coolNewApp`
* `cd coolNewApp/`
* `rm -rf .git/`
* `git init`
* `git config user.email "your@email.com"`
* `git config user.name "Your name"`
* `git add .`
* `git commit -m "Initial commit. Create new project from blank-project"`
* `pod install`
* Open coolNewApp XCode workspace file in XCode
* Open project settings and (1) change the team the app belongs to, (2) change target name (found in the right panel of XCode), (3) change bundle identifier. Quit XCode. 
* Open `Podfile` in a text editor. Edit the Podfile's "target" to the name of the new target name you set above ^^^. Run `pod install` again. Then, remove the old workspace file: `rm blank-project.xcworkspace`. Also, delete the LICENSE file if you're writing closed source: `rm LICENSE`
* Open `.swiftlint.yml` file and edit `blank-project` in `Sources` to name of your source directory.
* Open coolNewApp XCode workspace file again in XCode.
* Open project settings > General, scroll to bottom to view the list of all cocoapods/frameworks you have installed in app. Delete `Pods_blank-project.framework`. Quit XCode. 
* In finder, rename the blank-project source code directory to coolNewApp. Repeat for blank-projectTests and blank-projectUITests.
* Open coolNewApp XCode workspace file in XCode. Along left side where you view all of the files in your project, click on the blank-project group folder. Open the right panel of XCode and you will see a folder icon. Click this and choose the newly renamed folder you edited in the step above ^^^. Repeat this for the blank-projectTests and blank-projectUITests groups as well. Then, rename the group names in the left side panel (the folders with all of your code you were selecting and clicking on that folder icon in the right panel, those are called groups. They are not actually folders, just XCode organizers. Click on them and rename them to coolNewApp.)
* Open project settings > General in XCode again. Scroll to bottom to view the list of all cocoapods/frameworks installed. Remove Pods_coolNewApp.framework, then add it back. 
* Target > General in XCode. The middle where you usually enter your bundle identifier, it will have a button asking you to locate your Info.plist file. Choose coolNewApp/Info.plist. 
* Top left corner by the Play and Stop button. You see the schemas with name "blank-project". Click on it and go to "Manage schemas". You can now click on blank-project and rename it to coolNewApp. 
* Hold down option key on keyboard and click on the Play button. You can now select in the list what build version you want to run. I start with debug/dev. Go ahead and try to run on a device now. 
* Continue on with dev. Install Fabric for instance. 