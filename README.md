# Mobile Android Developer Learning Journey

# 1. Compose

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

#### Videos 
1. - [x] [The Jetpack Compose Beginner Crash Course for 2023 - speedy basics video](https://www.youtube.com/watch?v=6_wK_Ud8--0)
   - [ ] [Jetpack Compose](https://www.youtube.com/playlist?list=PLQkwcJG4YTCSpJ2NLhDTHhi6XBNfk9WiC)
2. - [ ] [Android Basics 2023](https://www.youtube.com/playlist?list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm)
        - [x] [Activities & the Activity Lifecycle](https://www.youtube.com/watch?v=SJw3Nu_h8kk)
              <details markdown='1'><summary>Learning</summary>
              <p>An activity is a container for one or multiple screens in your app OR a Unit of your app where users interact with
              <p> Activities contain info:
              - if it's currently active on the screen, if it's in the background, serve as an entry pointo your app e.g. if a use is coming from another app and click your app then an activity is a component that directly gets launched from that action
              
3. - [ ] [Android Fundamentals for Beginners](https://www.youtube.com/playlist?list=PLQkwcJG4YTCTq1raTb5iMuxnEB06J1VHX)
4. - [ ] [Gradle for Beginners](https://www.youtube.com/watch?v=o0M4f5djJTQ)
5. - [ ] [Convert Figma Designs to Jetpack Compose Code With This FREE Plugin](https://www.youtube.com/watch?v=byOmrmXG4yQ)
 
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

