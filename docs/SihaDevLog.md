Siha dev log
(dt-rush)
===

### Pomodoro 1: overview of open issues

Developer instructions - https://github.com/dt-rush/siha/issues/4
Describes the need for instructions for devs wanting to contribute
(environment setup, prereqs)

Data model / API - https://github.com/dt-rush/siha/issues/3
Describes the fact that we will use GraphQL for our data model / API layer

Investigate js frameworks for desktop + app - https://github.com/dt-rush/siha/issues/2
Describes the need to code the API / DB *and* UI only once
React native is selected for the framework

List of features - https://github.com/dt-rush/siha/issues/1
Describes an extensive list of desired features to exist in *one* app, the main Siha value proposition


### Pomodoro 2: environment setup

1. clone Siha repo
2. install [android studio](https://developer.android.com/studio)
3. `sudo apt update && sudo apt install android-sdk`
4. install [Android Command line tools](https://developer.android.com/studio#command-tools) (make sure to put them into the sdk root at `<sdk>/cmdline-tools/latest`)
5. add android studio dir to your PATH
6. add the following SDK dirs to your PATH:
```
export ANDROID_HOME=$HOME/Android/Sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/platform-tools
export PATH=$PATH:$ANDROID_HOME/cmdline-tools/latest/bin
```
7. open Siha directory as existing project in android studio
8. open Tools > AVD Manager, and "+ Create Virtual Device"
9. create a Galaxy Nexus device @ Release Name "R"
10. You may now use either CLI or android studio to develop the project
(CLI+vim is the way most in line with the laws of heaven)

### Pomodoro 3: environment testrun

Run `sdkmanager` (should be on path by by now)
Run `avdmanager list avd` (should show the android virtual device we created during environment setup)
Run `emulator -avd <NAME>` (in this case, it will be something like `Galaxy_Nexus_API_30`)
Open youtube app and look up "BTS film out official MV", enjoy for a little bit
Look up "Freddie Gibbs Gang Signs" and/or "Big Boss Rabbit"
Look up "Shackleton documentary"
We can now be assured that youtube is working, those are some good videos!!!

Ran into confusion having mixed up expo and react-native workflows. Spent time reading. We use expo.

### Pomodoro 4: environment setup

1. set emulator running
2. `expo start`
3. Now we're cookin'
4. Set up basic navigation/icons

## Signing off 2021-Apr-02

### Pomodoro 5: feature list expansion and comments

TODO

- [ ] Daily habit checkmark
- [ ] Timed daily habit checkmark
- [ ] Pomodoro timer w stats
- [ ] Daily journal entry
- [ ] Quantified daily journal entry
- [ ] Todo list
- [ ] Projects as tags
- [ ] Kanban view for project todos
- [ ] Search over all fields
- [ ] Tags
- [ ] Meta comments
- [ ] Links


