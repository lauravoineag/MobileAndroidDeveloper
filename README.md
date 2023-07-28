# Mobile Android Developer Learning Journey

Overview
[0. Android](https://github.com/lauravoineag/MobileAndroidDeveloper/blob/main/README.md#Android)

[1. Compose](https://github.com/lauravoineag/MobileAndroidDeveloper/blob/main/README.md#Compose)

[2.Kotlin](https://github.com/lauravoineag/MobileAndroidDeveloper/blob/main/README.md#Kotlin)

Android
1. - [ ] [Android Fundamentals](https://www.youtube.com/playlist?list=PLQkwcJG4YTCTq1raTb5iMuxnEB06J1VHX)

# 1.Compose

#### Learned while pairing:
- Make small changes frequently in the UI to see how components line up together (use Preview and SplitView) 
- Responsive design - design solutions in responsive ways - sizing the container is better than sizing the element - when you are looking at parent child relationship - you want a dynamic size for containers - e.g a button in a column - don't add size to button - size in the parent/column
- Design and Arhitecture -  Think about the responsibilities of what each class has - The Responsibilities will trigger all the output - OOP Principles
-  How to plan a UI ticket:
   * There are 3 catgories:
     1. Writing Componenets
     2. Adding Behaviour
     3. Adding Styling
   * You start writing in this order because you want to see visually how the components align together, to then be able to add the behaviour for them and finally the styling of components. You add the styling at the end because the behaviour might affect the styling and styling may then have to be refactored
- Golden module - We apply the principles of the team's defined “golden module” to all the existing and future modules in the codebase. The “golden module” is the pattern we apply to all feature modules.It’s not a module _itself_ but it shows us a set of principles we apply when we write a module.
- Two way binding = the same state - the same state that causes the state change will also trigger this on value change function which will update the state again
- State
  WHAT is the state? Declare the state. The main application has the responsibility of holding the state
  HOW does the state change?  Handler which holds the responsibility - still in main applicatin - updates the state
  WHEN is the state changing? It's the trigger/event which causes the state to change. It's the onClick event of the buttons.

#### Videos 
1. - [x] [The Jetpack Compose Beginner Crash Course for 2023 - speedy basics video](https://www.youtube.com/watch?v=6_wK_Ud8--0)
   - [ ] [Jetpack Compose](https://www.youtube.com/playlist?list=PLQkwcJG4YTCSpJ2NLhDTHhi6XBNfk9WiC)


[Full beginner roadmap:](https://www.youtube.com/watch?v=AhUL5tHF3uc)
         
2. - [ ] [Android Basics 2023](https://www.youtube.com/playlist?list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm)
      - [x] [Activities & the Activity Lifecycle](https://www.youtube.com/watch?v=SJw3Nu_h8kk)
              <details markdown='1'><summary>Learning</summary>
              <p> An activity is a container for one or multiple screens in your app OR a Unit of your app where users interact, generally it's the entry point of your application
              <p> Activities contain info:
              - if it's currently active on the screen, if it's in the background, serve as an entry pointo your app e.g. if a user is coming from another app and clicks your app then an activity is a component that directly gets launched from that action. More info [here](https://developer.android.com/guide/components/activities/activity-lifecycle)
              
      - [x] [Back Stack, Tasks & Launch Modes](https://www.youtube.com/watch?v=Z0AzoFOiH9c&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=2)
            <details markdown='1'><summary>Learning</summary>
            <p> **Backstack** - are a stack ofscreens/activities and how tese are arranged. Add Backstack when you open different applications - they get added to the backstack or remove backstack as soon as user clicks the back button or closes applications.</p>
             <img width="261" alt="Adding" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/c0e12432-6058-4d66-9422-d46a9219b440">
            <img width="261" alt="Screenshot 2023-07-24 at 08 46 06" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/2b4f6103-0001-497d-98dc-0f0c07184f22">
            <p> A **task** is the whole thing - represents the collection of multiple sceeens/activities that belong together</p>
            <img width="343" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/1780fefe-6f0a-48d2-adf0-6a13a56a173c">
            <p> Backstack is how these screens are arranged and the tasks combines all these screens into one unit. When you remove all backstacks from one task it stops being a task.</p>
            ![image](https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/b4949ce4-915a-4fa3-a2a0-99f8587a28a0)
            <p> **Launch modes** set the behaviour - what should happen when a new activity is pushed on the backstack.
            <p> **Standard** launchmode (don't change anything). When you open 2 links (2 different apps) in google chrome windows you generate 2 browse activities and they will be pushed to backstack. When we say Android open this activity, a new instance ofthat activity will be pushed on backstack.</p>
            <img width="614" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/2047557a-31b9-4dee-a987-29e0f89c21db">
            <p> **Single Top** launchmode The user goes from another app to Chrome - if there is an existing app with an activity launched that we want then we won't add another activity on top but send the user to existing one. You want the user to go back to the same activity.
            <p>**Single Task** launchmode single task assigned to Browser Activity (via Bookmark) it will make sure that new instances will be launched inside a completely separate task.
            <p> Why not send to already existing activity? You only want to open a specific link(LinkedIn) and when the user goes back they want to go back to their activity(LinkedIn) and not Bookmark activity. The already existing taks(Browser Activity) has already existing backstack & if user goes back they will not go back to where they want(their initial app- LinkedIn) but back to Bookmark activity.</p>
            <img width="918" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/5b85e44c-f532-41c9-a1f0-ea1bfa829589">
            <p>**Single Instance** launchmode will also launch a different task independent of the previous active taks but the difference is this new Browser activity which was opened is completely isolated so inside it you are not allowed to open any other activities (payment app paypal)and the user cannot interfere with other apps while on it(security risk)</p>
 
      - [x] [ViewModels & Configuration Changes](https://www.youtube.com/watch?v=9sqvBydNJSg&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=5)
            
          <details markdown='1'><summary>Learning</summary>
          <p> **MVVM **
        <p> 1. Generally, the View Model's job is to take the raw data from Model and bring it into a new format easy to display in the UI.The View Model will convert data from Model -> into a format that UI understands and as soon as that happens the View Model will then automatically notify the UI that there is a change so that the UI can update and show new info.
        <p> Whenever something has to do with Real Data Source(DB) VM sends new data to Model the Model saves it and notifies the UI again. 
        <p> 2. No Model! - VM has the responsibility to chage the state and notify UI - When user clicks to change bakground colour we call VM. (UI -> sends UserAction to ViewModel so the VM can react to it) that doesn't need the Model since the UI action would be the button click, the VM updates the state that the background colour changed and notifies the UI so the UI can show the background colour. VM receives a User Action/UI Action/Event from the UI(View) -Button Click,Swipe different page</p>
          <img width="1124" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/d2b5ad36-dc14-49e7-b024-759aa24fbfe6">
        <p> Configuration change - screen rotation, user changes language, theme - app needs to update all colours.How Android deals with these changes is by re-creating the whole activity(current instace of activity distroyed- lifecycle moves to onDestroyed state and when the rotation finished it will start with a new activity). The VM will also be re-created.
        <p> Eg below where on screen rotation the background is not changed </p>
        <img width="573" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/9f59460e-a900-4679-820a-0609d9ab8507">
          <img width="573" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/7169cd75-3396-4d04-9338-61e40bf35951">
          <p>Eg below where on screen rotation the background is changed
          Inheriting from ViewModel it will create a component which will outlive the life cycle of its screen(activity). The activity has a lifecycle that ends when we rotated the device then this VM that it inherits from will outlive and won't be distroyed when the activity will be distroye. It will be distroyed when use pops the activity from the backstack(back button)</p>
          <img width="573" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/eb1a8034-97cf-4462-921b-5684a5095101">
          <p>The VM won't be destroyed because of configuration changes we need to use the Android way of initialising the View Models</p>
          <img width="738" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/6ed0c59f-deb4-4035-9d66-d70e12f83ae7">
          <p> View Model factory - a class that defines how our viewModel instance is to created with the Android ViewModel</p>
          <img width="800" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/6660238b-6370-4ee6-abaf-e73444e0ae5e">

     - [x] [Text Fields - UX With Material3](https://www.youtube.com/watch?v=ZERIxmBYP-U)

3. - [ ]  Android framework [Platform arhitecture](https://developer.android.com/guide/platform)           
4. - [ ] [Android Fundamentals for Beginners](https://www.youtube.com/playlist?list=PLQkwcJG4YTCTq1raTb5iMuxnEB06J1VHX)
5. - [ ] [Gradle for Beginners](https://www.youtube.com/watch?v=o0M4f5djJTQ)
6. - [ ] [Convert Figma Designs to Jetpack Compose Code With This FREE Plugin](https://www.youtube.com/watch?v=byOmrmXG4yQ)

https://developer.android.com/samples
 List
 Android SDK
AndroidManifest.xml - and they all (broadcast receiver doesn't have to be) are defined in an applications AndroidManifest.xml file too
eg.
<manifest>
   <application ...> <- android.app.Application definition
      <activity ...> <- android.app.Activity definition
      <receiver ...> <- Broadcast receiver definition
      <service ...> <- Service definition
      <provider ...> <- Content provider definition
   </application>
</manifest>

What is vital to learn -   knowing the application level components (Activity, Application, Service, Broadcast Receiver, Content Provider)
[Application](https://developer.android.com/reference/android/app/Application)
[Services](https://developer.android.com/guide/components/services)
[Broadcast receiver](https://developer.android.com/guide/components/broadcasts)
[Content Provider](https://developer.android.com/guide/topics/providers/content-providers#:~:text=Content%20providers%20are%20the%20standard,as%20illustrated%20in%20figure%201)

#### Codelabs 
- [ ] [All](https://developer.android.com/courses/fundamentals-training/toc-v2)
- [ ] [Codelab basics](https://developer.android.com/codelabs/jetpack-compose-basics#12)

#### MAD skills videos -  do Android basics code labs before watching these
- [ ] Kotlin in Android - [****](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc98e0f5ZbsgB63MdjZTFgsy)
 
 ##### Compose:
- [ ] [****](https://developer.android.com/courses/jetpack-compose/course?gclid=EAIaIQobChMIlKnfpeCcgAMVQotoCR2BfggUEAAYASAAEgLyfvD_BwE&gclsrc=aw.ds)
- [ ] [****](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc-CG9riunK996aI6cRhXFDC)
- [ ] [****](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc94tpHND8pW8Qt8ZfT1a4cq)

 ##### Architecture Videos:
- [ ] MVVM Shopping List - [****](https://www.youtube.com/playlist?list=PLQkwcJG4YTCT0RouHZ6sQlE4JE6VyD2zO)
- [ ] [****](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc8GZWCbUm3tBXKeqIi3rcVX)
- [ ] MVVM NewsApp, Retrofit, Room, Coroutines, Navigation Components [****](https://www.youtube.com/playlist?list=PLQkwcJG4YTCRF8XiCRESq1IFFW8COlxYJ)
- [ ] [****](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc8GZWCbUm3tBXKeqIi3rcVX)

####  Architecture Intro: 
- [ ] Guide to app https://developer.android.com/topic/architecture https://developer.android.com/topic/architecture#unidirectional-data-flow
-  Coding patterns - overview of software and Architecture 
- [ ] https://developer.android.com/guide/components/activities/intro-activities
- [ ] https://developer.android.com/topic/libraries/architecture/viewmodel
- [ ] https://developer.android.com/guide/fragments
- [ ] https://developer.android.com/topic/architecture
- [ ] https://developer.android.com/topic/libraries/architecture/viewmodel
- [ ] https://medium.com/swlh/understanding-mvvm-architecture-in-android-aa66f7e1a70b

##### Android Projects
- [ ] [****](https://www.youtube.com/playlist?list=PLQkwcJG4YTCSSow0ulsj-kIc6drYG_D0E)
- [ ] Pokédex App with Jetpack Compose [****](https://www.youtube.com/playlist?list=PLQkwcJG4YTCTimTCpEL5FZgaWdIZQuB7m)
- [ ] MVVM Spotify Clone [****](https://www.youtube.com/playlist?list=PLQkwcJG4YTCT-lTlkOmE-PpRkuyNXq6sW)
- [ ] 
 ##### Extras (These are only if you are especially interested)
- [ ] Gradle (how we build the app, just this one video) [****](https://www.youtube.com/watch?v=GjPS4xDMmQY)
- [ ] Navigation - [****](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc9VpBMZUS9geQtc5RJ2RsUd)
- [ ] More navigation - [****](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc-vin7SvgoaR6wu24sAw-sE)
- [ ] Back Stack - [****](https://www.youtube.com/watch?v=MvIlVsXxXmY)

#### UI reading 
- [ ] Component Design - [****](https://atomicdesign.bradfrost.com/table-of-contents/)

#### Android fundamentals
- [ ] Android Life cycle [****](https://www.javatpoint.com/android-life-cycle-of-activity)
- [ ] [****](https://www.youtube.com/watch?v=pcnnbjAAIkI&t=9s)
- [ ] DB & Cloud Stuff


#### Testing:
- [ ] Testing in Android [****](https://www.youtube.com/playlist?list=PLQkwcJG4YTCSYJ13G4kVIJ10X5zisB2Lq)
- [ ] https://developer.android.com/jetpack/compose/testing-cheatsheet
- [ ] https://developer.android.com/jetpack/compose/testing
- [ ] https://developer.android.com/codelabs/jetpack-compose-testing?authuser=1#1
- [ ] https://youtu.be/kdwofTaEHrs

#### Components:
- [ ] Lazy grid [****](https://youtu.be/eC-hNDgUd1Y)

#### Random
- [ ] use a screenreader https://support.google.com/accessibility/android/answer/6007100?hl=en-GB
- [ ] Git branching https://learngitbranching.js.org/
- [ ] Accessibility https://developer.android.com/jetpack/compose/accessibility?authuser=1
- [ ] AWS Essential Course
- [ ] Remote config https://www.youtube.com/watch?v=pcnnbjAAIkI  https://firebase.google.com/docs/remote-config/get-started?platform=ios

* Remote config the problem (why)
    - To be able to change the way apps look in terms of design and behave on the users' phones without needing them to update the app on one of the app stores.

* How we use it
    - Every version of the apps we put on the stores has it's own version number - i.e. 1.150.0, 1.151.0, 1.151.1 etc.
We put a unique copy of config up on the web for each version we release. Each version of the app essentially looks for the config for it's own app version. Android version 1.151.1 will look for something like android - 1.151.1.json on the web.

* The benefit
    - Each version of the app that gets released to the store has different behaviour and capabilities and therefore needs its own config. e.g. we can't enable Top Nav for a version of the app in live that doesn't contain the code for Top Nav, therefore the config for that version won't contain an "enableTopNav" config.
We can turn things on remotely - but we can also turn things off remotely if they go wrong! So, if we were turn on a new feature this week for the latest version and suddenly there were a bunch of crashes, we can turn it back off again - much less catastrophic of having to kill a version of the app.

    - Remote config does allow us to kill a version of the app though! E.g. a bug is written in version 1.160.0 of the app, that meant that the app sent 1000000 requests to API service an hour and it wasn't behind a feature flag like the new feature, then we really don't want that version of the app to continue being used. We can remotely say "turn the kill switch on for version 1.160.0" and then any users on that version will see a message in the app saying "you need to update the app in order to carry on using our app" and API service(a different department who is responsible for supplying information relevant to our new feature) won't be in so much trouble.

    - Seeing this in a another way, it's just like any back-end service, the app makes a request for data over HTTP and the server responds. If the API service Url was moving to a new location, we can just edit the remote config file to reflect that new location. If we didn't have remote config, and the Url had been hard coded into the app, then we would need to do a new release of the app to change the url and kill the old versions. Mobile is different to web in that we have many versions of the application live at any one time as people are free to take updates as and when they choose. This means we have to be able to reconfigure the application after it has been released and remote config is our mechanism to do that.


# 2. Kotlin


#### Android Kotlin courses
- [ ] [Kotlin from newbie to pro](https://www.youtube.com/playlist?list=PLQkwcJG4YTCRSQikwhtoApYs9ij_Hc5Z9)
- [ ] https://developer.android.com/courses/android-basics-kotlin/course
- [ ] https://developer.android.com/kotlin
- [ ] KOTLIN NEWBIE TO PRO https://www.youtube.com/playlist?list=PLQkwcJG4YTCRSQikwhtoApYs9ij_Hc5Z9

- [x]  Pluralsight (one course - 3 days;  course 2 - 3 days)  - 6 days of Pluralsight - Kotlin Fundamentals by Kevin Jones - done(2 weeks) https://app.pluralsight.com/channels/details/f7146668-d19c-4661-949c-cffa6a6556f5
    Kotlin Fundamentals by Kevin Jones
- [x] Exercism - Katas to learn Kotlin (1 week of kata only) but ongoing after - one a week - https://exercism.org/tracks/kotlin

# 3. Ticket stuff
- [x] Swimming lanes https://www.oldstreetsolutions.com/jira-swimlanes-agile-boards
- [x] 3 amigos - kick off 
    - It's basically the last chance saloon to question if we should be doing the work, if we do the work how we'll do it and if the work is done how we'd test it. 
    - It's a meeting that is used to ensure everyone understands what a ticket's purpose is. The three amigos (3 friends)is broken down into the following departments: delivery/project (like product owner or delivery manager and UX), someone from test and someone from dev. At the end of the meeting everyone should be 100% certain on what the output of the ticket will be (a definition of done should have already been met in sprint planning and backlog refinement). It's really useful just to make certain that before you start a ticket, the world hasn't shifted in any big way and that testers will understand how to test what it is you're doing and product understand what the main value will be too.
    - Sometimes something will be planned in (usually integrating with another team's work) and we'll find out "actually they're not ready for us to integrate, I had a chat with the team this morning!"
    - or "yeah the way we thought we'd implement that won't work because the library has a bug in it"
    - or "we won't be able to test it because the test environment isn't ready yet"
    - all of those things would be rare for one single person to have knowledge of
  
 - [ ] CI/CD
 - [ ] CI is continuous integration - GIT management - 
"When I commit my code to a branch and intend to merge it (create a PR) I want all the tests we've got to execute against it to make sure the changes are safe" and "When my changes are merged into main, I want to make sure that the resultant code can successfully generate a build artifact (APK, IPA etc) and all the tests pass"
The idea is, if you have a good CI setup, you can have confidence that what you've got in `main` is always shippable! This isn't always strictly true in a lot of projects you encounter, but it's definitely the target.
To keep main shippable, people will often use 'feature toggles' or 'feature switches' or 'feature flags', which is a way of shipping an experimental or incomplete feature, without it being accessible. So tom said in stand up "I'm working on downloading, I'm not worried because it's behind a feature flag" meaning he's not worried about it being released because no one can access it

 - [ ] CD -Continuous Delivery -  from releasing code to how the user gets it 

The idea that every single commit made to main is not only releasable, but is also released! The argument is: "If you have sufficient automated testing, it should be possible to continuously deliver the latest version of your software as soon as it is available".
In practice, people are super worried about that, and it only really works in an environment where you can push updates to users (e.g. websites or services) whilst mobile development is a pull model, where someone needs to go to the store and tap on update to get any changes (boo).
We may use CD to publish potential releases to the Alpha/Beta tracks of Google Play.

# 3. Other platforms for learning Language:
 ##### Practice Language Code wars - Katas to learn Kotlin
- https://www.codewars.com/
- https://play.kotlinlang.org/koans/overview

 ##### Other resources
- https://developer.android.com/kotlin/style-guide?authuser=1
- https://developer.android.com/studio/projects?authuser=1
- https://developer.android.com/courses/android-basics-kotlin/android-basics-kotlin-vocab?authuser=1

  ##### Course syllabus Jetpack Compose:
  https://www.udemy.com/course/mastering-jetpack-compose/
- Kotlin Basics and OOP
  -- The Basics
  -- OOP
  -- Data Structures
  -- High Order Functions
- Composables
  -- Basics (Buttons, Images, Texts, TextField)
  -- More Composables (Radio Button, Checkbox, Indicators)
  -- Layouts(Box, Row, Column, Scaffolds, Cards)
  -- Lazy Composables (Lazy Col, Rows, Grids)
- State Management
- Navigation
- MVVM Arhitecture
   -- MVVM Concept
   -- ROOM Database
   -- Retrofit - Fetching Data from APi

 ##### Inspiration for project designs:
https://dribbble.com/shots
https://daringfireball.net/projects/markdown/syntax#overview
