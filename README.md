# Mobile Android Developer Learning Journey

# 1. Compose

#### Learned while pairing:
- make small changes frequently in the UI 
- responsive design - design solutions in responsive ways -sizing the container is better than sizing the element - when you are looking at parent child relationship - you want a dynamic size for containers - e.g a button in a column- don't add size to button - add the size in the parent/column 


#### Codelabs 
- [ ] All https://developer.android.com/courses/fundamentals-training/toc-v2
- [ ] Codelab basics https://developer.android.com/codelabs/jetpack-compose-basics#12

#### MAD skills videos -  do Android basics code labs before watching these

- [ ] Kotlin in Android - https://www.youtube.com/playlist?list=PLWz5rJ2EKKc98e0f5ZbsgB63MdjZTFgsy
 
 ##### Compose:
- [ ] https://www.youtube.com/playlist?list=PLWz5rJ2EKKc-CG9riunK996aI6cRhXFDC
- [ ] https://www.youtube.com/playlist?list=PLWz5rJ2EKKc94tpHND8pW8Qt8ZfT1a4cq

 ##### Architecture:
- [ ] https://www.youtube.com/playlist?list=PLWz5rJ2EKKc8GZWCbUm3tBXKeqIi3rcVX

 ##### Extras (These are only if you are especially interested)
- [ ] Gradle (how we build the app, just this one video) https://www.youtube.com/watch?v=GjPS4xDMmQY
- [ ] Navigation - https://www.youtube.com/playlist?list=PLWz5rJ2EKKc9VpBMZUS9geQtc5RJ2RsUd
- [ ] More navigation - https://www.youtube.com/playlist?list=PLWz5rJ2EKKc-vin7SvgoaR6wu24sAw-sE
- [ ] Back Stack - https://www.youtube.com/watch?v=MvIlVsXxXmY

#### Videos 
- [x] Compose basics video - speedy basics video - https://www.youtube.com/watch?v=6_wK_Ud8--0

#### Arhitecture
https://www.youtube.com/playlist?list=PLWz5rJ2EKKc8GZWCbUm3tBXKeqIi3rcVX

#### UI reading 
- [ ] Component Design - https://atomicdesign.bradfrost.com/table-of-contents/

#### Android fundamentals
- [ ] Android Life cycle https://www.javatpoint.com/android-life-cycle-of-activity
- [ ] Remote configuration
- [ ] DB & Cloud Stuff

####  Architecture 
- [ ] Guide to app https://developer.android.com/topic/architecture https://developer.android.com/topic/architecture#unidirectional-data-flow
-  Coding patterns - overview of software and Architecture 
- [ ] https://developer.android.com/guide/components/activities/intro-activities
- [ ] https://developer.android.com/topic/libraries/architecture/viewmodel
- [ ] https://developer.android.com/guide/fragments
- [ ] https://developer.android.com/topic/architecture
- [ ] https://developer.android.com/topic/libraries/architecture/viewmodel
- [ ] https://medium.com/swlh/understanding-mvvm-architecture-in-android-aa66f7e1a70b

#### Testing:
- [ ] https://developer.android.com/jetpack/compose/testing-cheatsheet
- [ ] https://developer.android.com/jetpack/compose/testing
- [ ] https://developer.android.com/codelabs/jetpack-compose-testing?authuser=1#1
- [ ] https://youtu.be/kdwofTaEHrs

#### Components:
- [ ] Lazy grid https://youtu.be/eC-hNDgUd1Y

#### Random
- [ ] use a screenreader https://support.google.com/accessibility/android/answer/6007100?hl=en-GB
- [ ] Git branching https://learngitbranching.js.org/
- [ ] Accessibility https://developer.android.com/jetpack/compose/accessibility?authuser=1
- [ ] AWS Essential Course
- [ ] Remote config


# 2. Kotlin

#### Android Kotlin courses
- [ ] https://developer.android.com/courses/android-basics-kotlin/course
- [ ] https://developer.android.com/kotlin

- [x]  Pluralsight (one course - 3 days;  course 2 - 3 days)  - 6 days of Pluralsight - Kotlin Fundamentals by Kevin Jones - done(2 weeks) https://app.pluralsight.com/channels/details/f7146668-d19c-4661-949c-cffa6a6556f5
    Kotlin Fundamentals by Kevin Jones
- [x] Exercism - Katas to learn Kotlin (1 week of kata only) but ongoing after - one a week - https://exercism.org/tracks/kotlin

# 3. Ticket stuff
- [x] Swimming lanes https://www.oldstreetsolutions.com/jira-swimlanes-agile-boards
- [x] 3 amigos - kick off 
- last chance saloon to question if we should be doing the work, if we do the work how we'll do it and if the work is done how we'd test it 
- is a meeting that is used to ensure everyone understands what a ticket's purpose is. The three amigos (3 friends) represent someone from delivery/project (like product owner or delivery manager), someone from test and someone from dev. At the end of the meeting everyone should be 100% certain on what the output of the ticket will be (a definition of done should have already been met in sprint planning and backlog refinement). It's really useful just to make certain that before you start a ticket, the world hasn't shifted in any big way and that testers will understand how to test what it is you're doing and product understand what the main value will be too
- sometimes something will be planned in (usually integrating with another team's work) and we'll find out "actually they're not ready for us to integrate, I had a chat with the team this morning!"
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

# 3 . Other platforms for learning Language:

 ##### Practice Language Code wars - Katas to learn Kotlin
- https://www.codewars.com/
- https://play.kotlinlang.org/koans/overview

 ##### Other resources
- https://developer.android.com/kotlin/style-guide?authuser=1
  

    https://developer.android.com/studio/projects?authuser=1
https://developer.android.com/courses/android-basics-kotlin/android-basics-kotlin-vocab?authuser=1

