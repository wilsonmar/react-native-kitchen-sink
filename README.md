This repository contains code for a cross-platform mobile app written using
<a target="_blank" href="http://facebook.github.io/react-native/"> 
React-Native from Facebook</a>.

Unlike other sample "boilerplate" and "starter" apps on Github
that just throws a string to a blank screen,
this repo provides a full experience:

   * Video splash screen that works offline.
   * Account registration.
   * Login via Facebook, Twitter, Google, Github.
   * Two-factor authentication with signing and data encryption
   * API calls to Salesforce, Twillo for SMS, and various other data sources
   * User preferences (color, greeting, etc.)
   * A "Kitchen Sink" of known GUI elements
     (color picker, menus, lists, spinners, carosels, etc.)
   * Shopping cart for Amazon, Walmart, 


<strong>Developers</strong> can leverage this to focus on content for their own app,
not waste time on plumbing code.

Courses that explain how to program explain this source code.
In fact, seminars and support is how we fund this app's development.

<strong>Testers</strong> would especially appreciate this app because it contains
features not available in other apps (on purpose, anyway), such as:

   * A button that crashes the app, useful for testing loggging.
   * Tracking of every call with how long the round-trip took.
   * And other features you suggest.

This app enables work on Ensd-to-end integration scripts even before your developers produce custom code.

Additional information include:

* <a target="_blank" href="https://github.com/jondot/awesome-react-native">
  An "awesome" type curated list of React Native components, news, tools, and learning material</a>

### Example apps:

* https://github.com/facebook/react-native/tree/master/Examples
* https://github.com/alinz/example-react-native-redux
* https://github.com/christopherdro/react-native-sudoku

## Setup iOS
https://facebook.github.io/react-native/docs/getting-started.html#content

## Setup Android

### Setup 

0. `brew install android-sdk`
0. Open a new Terminal window to invoke `android`. A green ball GUI should appear.
0. Install SDK Tools, Platform-tools, Build-tools.
0. Uncheck Android 6.0 (API 23) to be selective.
0. Check its SDK Platform, Intel x86 Atom_64 and Atom System Images.
0. In Extras: Android Support Repository.
0. Click "Install all 6 packages".
0. Click "Accept" then "Install".

### Setup Gradle daemon
 A daemon is a computer program that runs as a background process, rather than being under the direct control of an interactive user. 

0. Use a browser to open https://www.udacity.com/course/gradle-for-android-and-java--ud867
   and take the free video class.

   NOTE: Gradle one-day on-line classes are $700 each.

   * http://gradle.org/getting-started-android/
   * https://docs.gradle.org/2.9/userguide/gradle_daemon.html


### Setup Genymotion emulators for developers:
These steps you'll only need to done once:

0. Signup for a Personal Use account at http://Genymotion.com/ 
0. Click the confirmation email link.
0. At https://www.genymotion.com/pricing-and-licensing/ click the Individual tab and Get Started.
0. Download Genymotion-2.6.0.dmg (or whatever version).
0. Use Finder in your Downloads folder, open the .dmg file.
0. Drag the Genymotion icon and drop it on the Applications folder.
0. Repeat for the Genymotion shell.
0. Click the red x to dismiss the dialog.
0. PROTIP: In Finder, move to trash the .dmg file so it doesn't clutter up your hard drive.
0. In Finder, in the Go menu scroll to click open Genymotion. 
0. Add a virtual device. NOTE: Not a large number of choices.
   See the Perfecto Mobile report for what is popular.

0. Enable emulator Systrace: `brew install trace2html`.

### Emulators for developers:
These steps you'll be repeating:

0. After `npm install -g react-native-cli`, invoke an ios emulator within a repo:

   ```
   react-native run-ios
   ```

   Expect a lot of messages while it builds.
   A new terminal window pops up automatically.
   
0. In Genymotion, click Start device.

0. Navigate to the Awesome app folder.
0. Invoke an Android emulator:

   ```
   react-native run-android
   ```

  NOTE: According to Facebook's https://www.npmjs.com/package/react-native
  (at time of this writing)
  Supported operating systems are >= Android 4.1 (API 16) and >= iOS 7.0.

0. To bring up the developer menu press ⌘+M
0. Open index.android.js in your text editor of choice and edit some lines.
0. Press the menu button (F2 by default, or ⌘-M in Genymotion) 
   and select Reload JS to see your change.
0. To see your app's logs, run `adb logcat *:S ReactNative:V ReactNativeJS:V`.

  PROTIP: Keep track of memory usage at each stage of developerment
  so you know how resources increase with each feature added.

0. Press Command+D for the menu.
0. Select 
0. Stop the simulator from the terminal by control+C.
0. Quit the simulator by right-clicking on the simulator icon and selecting Quit.

   PROTIP: Delete trace files to keep your disk drive from overfilling.

0. If tracing occurred, open a new terminal to view then delete log files.

   ```
   cd /tmp
   rm -rf *.json
   ```

* https://rnplay.org/ 
  Paste the code in and React Native Playground simulates iOS and Android devices online,
  across multiple React Native versions. Open sourced at
  https://github.com/rnplay/rnplay-native/blob/master/package.json#L10-L25

* https://tonicdev.com/npm/react-native also runs code online.

* https://github.com/Shrugs/react-native-snippets for sublime text
* http://www.blackdogfoundry.com/blog/migrating-ios-app-through-multiple-environments/
* http://browniefed.com/react-native-animation-book/

### Basics:

* https://github.com/adamjmcgrath/react-native-simple-auth for social account authentication within iOS
* https://github.com/calebd/SimpleAuth at http://simpleauth.io/

* https://github.com/walmartreact/react-native-platform-visible
* https://github.com/oblador/react-native-vector-icons
* https://github.com/stefalda/ReactNativeLocalization
* https://github.com/darylrowland/react-native-remote-push

* https://github.com/TylerLH/react-native-timeago

* https://github.com/joeferraro/react-native-env Access environment variables from React Native 
* https://github.com/lwansbrough/react-native-google-analytics
* https://github.com/joeferraro/react-native-cookies

* https://github.com/almost/react-native-sqlite
* https://github.com/andpor/react-native-sqlite-storage
* https://github.com/aerofs/react-native-auto-updater

### Design:

* https://github.com/react-native-material-design/react-native-material-design

### UI Elements:

* https://github.com/mastermoo/react-native-action-button if you like Google's Material Design flotating button on the lower right.
* https://github.com/APSL/react-native-button

* https://github.com/umhan35/react-native-search-bar
* https://github.com/FaridSafi/react-native-gifted-listview
* https://github.com/alinz/react-native-dropdown
* https://github.com/ArnaudRinquin/react-native-radio-buttons

* https://github.com/lelandrichardson/react-native-parallax-view
* https://github.com/aksonov/react-native-tabs
* https://github.com/sunnylqm/react-native-storage
* https://github.com/react-native-fellowship/react-native-navbar
* https://github.com/react-native-fellowship/react-native-side-menu

* https://github.com/walmartreact/curved-carousel
* https://github.com/nick/react-native-carousel
* https://github.com/appintheair/react-native-looped-carousel


* https://github.com/leecade/react-native-swiper
* https://github.com/tomauty/react-native-chart
* https://github.com/lelandrichardson/react-native-maps
* https://github.com/aksonov/react-native-tableview
* https://github.com/johanneslumpe/react-native-selectablesectionlistview
* https://github.com/alinz/react-native-tabbar

* https://github.com/maxs15/react-native-spinkit

### Miniapps:

* https://github.com/rt2zz/react-native-contacts
* https://github.com/joemaddalone/react-native-todo
* https://github.com/christopherdro/react-native-calendar

* https://github.com/jeanregisser/react-native-slider
* https://github.com/benoitvallon/react-native-nw-react-calculator
* https://github.com/paramaggarwal/react-native-youtube

* https://github.com/facebook/react-native-applinks enables use of Facebook http://applinks.org/
* https://github.com/tabalt/ReactNativeNews
* https://github.com/christopherdro/react-native-rss-reader

* https://github.com/appintheair/react-native-buyscreen
* https://github.com/thewei/react-native-store
* https://github.com/walmartlabs/react-native-starter 
    A simple React Native starter project that uses the Walmart API to return and display product data from a barcode scan. iOS only.

* https://github.com/jsphkhan/ReactNativeExamples
* https://github.com/taskrabbit/ReactNativeSampleApp

* https://github.com/doefler/react-native-social-share Use the iOS native Twitter and Facebook share popup in react native 
* https://github.com/naoufal/react-native-activity-view  React Native Activity View is a React Native library for displaying iOS share and action sheets.

react-native-activity-view

### Mobile hardware:

* https://github.com/walmartreact/react-native-orientation-listener is the most starred on http://walmartlabs.com/
* https://github.com/transistorsoft/react-native-background-geolocation
* https://github.com/andreaskeller/react-native-audioplayer
* https://github.com/frostney/react-native-ibeacon
* https://github.com/timfpark/react-native-location
* https://github.com/jsierles/react-native-audio ( target filename must have an extension of '.caf')
* https://github.com/lwansbrough/react-native-camera
* https://github.com/brentvatne/react-native-video
* Take photo
* https://github.com/marcshilling/react-native-image-picker

