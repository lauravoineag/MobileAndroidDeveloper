# Mobile Android Developer Learning Journey

[Shuhari](https://en.wikipedia.org/wiki/Shuhari) 

Overview

[0. Android](https://github.com/lauravoineag/MobileAndroidDeveloper/blob/main/README.md#Android)

[1. Compose](https://github.com/lauravoineag/MobileAndroidDeveloper/blob/main/README.md#Compose)

[2. Kotlin](https://github.com/lauravoineag/MobileAndroidDeveloper/blob/main/README.md#Kotlin)

Organising:
[Android Dev- Full Path Planning](https://www.youtube.com/watch?v=AhUL5tHF3uc)

- [ ] [Android Fundamentals](https://www.youtube.com/playlist?list=PLQkwcJG4YTCTq1raTb5iMuxnEB06J1VHX)*


#### Learned while pairing:
<details>
<summary>Useful information</summary>
  
* Make small changes frequently in the UI to see how components line up together (use Preview and SplitView)
  
* Responsive design - design solutions in responsive ways - sizing the container is better than sizing the element - when you are looking at parent child relationship - you want a dynamic size for containers - e.g a button in a column - don't add size to button - size in the parent/column
  
* Design and Arhitecture -  Think about the responsibilities of what each class has - The Responsibilities will trigger all the output - OOP Principles
  
* How to plan a UI ticket in this order:
  - Writing Componenets
  - Adding Behaviour
  - Adding Styling
  
* You start writing in this order because you want to see visually how the components align together, to then be able to add the behaviour for them and finally the styling of components. You add the styling at the end because the behaviour might affect the styling and styling may then have to be refactored
  
* Golden module - We apply the principles of the team's defined “golden module” to all the existing and future modules in the codebase. The “golden module” is the pattern we apply to all feature modules.It’s not a module _itself_ but it shows us a set of principles we apply when we write a module.
  
* Two way binding = the same state - the same state that causes the state change will also trigger this on value change function which will update the state again
  
* State
  - WHAT is the state? Declare the state. The main application has the responsibility of holding the state
  - HOW does the state change?  Handler which holds the responsibility - still in main applicatin - updates the state
  - WHEN is the state changing? It's the trigger/event which causes the state to change. It's the onClick event of the buttons.
</details>

#### Lessons:
<details>
<summary>Useful information</summary>
  * If you create a second activity you need to register it in the Activity Manifest (see Intent)
</details>

# Compose

#### Videos 
1. - [x] [The Jetpack Compose Beginner Crash Course for 2023 - speedy basics video](https://www.youtube.com/watch?v=6_wK_Ud8--0)
  2. - [ ] [Jetpack Compose Basics](https://www.youtube.com/playlist?list=PLQkwcJG4YTCSpJ2NLhDTHhi6XBNfk9WiC)*
       - [x] [Creating your first Jetpack Compose App - Part1](https://www.youtube.com/watch?v=cDabx3SjuOY&list=PLQkwcJG4YTCSpJ2NLhDTHhi6XBNfk9WiC&index=1)
       - [x] [Rows, Columns & Basic Sizing - Android Jetpack Compose - Part 2](https://www.youtube.com/watch?v=rHKeRWK3zL4&list=PLQkwcJG4YTCSpJ2NLhDTHhi6XBNfk9WiC&index=2)
       - [x] [Modifiers - Android Jetpack - Part 3](https://www.youtube.com/watch?v=XCuC_p3E0qo&list=PLQkwcJG4YTCSpJ2NLhDTHhi6XBNfk9WiC&index=4)
       - [x] [Creating an image Card](https://www.youtube.com/watch?v=KPVoQjwmWX4&list=PLQkwcJG4YTCSpJ2NLhDTHhi6XBNfk9WiC&index=4)
       - [x] [Styling Text](https://www.youtube.com/watch?v=nm_LNJWHi9A&list=PLQkwcJG4YTCSpJ2NLhDTHhi6XBNfk9WiC&index=5)
   - [ ] [Jetpack Compose](https://www.youtube.com/playlist?list=PLQkwcJG4YTCSpJ2NLhDTHhi6XBNfk9WiC)


[Full beginner roadmap:](https://www.youtube.com/watch?v=AhUL5tHF3uc)
         
3. - [ ] [Android Basics 2023](https://www.youtube.com/playlist?list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm)
      - [x] [Activities & the Activity Lifecycle](https://www.youtube.com/watch?v=SJw3Nu_h8kk)
            <details><summary>Summary</summary>
           * An activity is a container for one or multiple screens in your app OR a Unit of your app where users interact, generally it's the entry point of your app
           * Activities contain info: if it's currently active on the screen, if it's in the background, serve as an entry pointo your app e.g. if a user is coming from another app and clicks your app then an activity is a component that directly gets launched from that action. More info [here](https://developer.android.com/guide/components/activities/activity-lifecycle) 
            
      - [x] [Back Stack, Tasks & Launch Modes](https://www.youtube.com/watch?v=Z0AzoFOiH9c&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=2)
            <details><summary>Summary</summary>
           * **Backstack** - are a stack ofscreens/activities and how tese are arranged. Add Backstack when you open different applications - they get added to the backstack or remove backstack as soon as user clicks the back button or closes applications.
           <img width="261" alt="Adding" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/c0e12432-6058-4d66-9422-d46a9219b440">
           <img width="261" alt="Screenshot 2023-07-24 at 08 46 06" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/2b4f6103-0001-497d-98dc-0f0c07184f22">
           
           * A **task** is the whole thing - represents the collection of multiple sceeens/activities that belong together.
            <img width="343" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/1780fefe-6f0a-48d2-adf0-6a13a56a173c">
           * Backstack is how these screens are arranged and the tasks combines all these screens into one unit. When you remove all backstacks from one task it stops being a task.
            ![image](https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/b4949ce4-915a-4fa3-a2a0-99f8587a28a0)

           * **Launch modes** set the behaviour - what should happen when a new activity is pushed on the backstack.
           * **Standard** launchmode (don't change anything). When you open 2 links (2 different apps) in google chrome windows you generate 2 browse activities and they will be pushed to backstack. When we say Android open this activity, a new instance ofthat activity will be pushed on backstack.
            <img width="614" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/2047557a-31b9-4dee-a987-29e0f89c21db">
           * **Single Top** launchmode The user goes from another app to Chrome - if there is an existing app with an activity launched that we want then we won't add another activity on top but send the user to existing one. You want the user to go back to the same activity.
           * **Single Task** launchmode single task assigned to Browser Activity (via Bookmark) it will make sure that new instances will be launched inside a completely separate task.
           * Why not send to already existing activity? You only want to open a specific link(LinkedIn) and when the user goes back they want to go back to their activity(LinkedIn) and not Bookmark activity. The already existing taks(Browser Activity) has already existing backstack & if user goes back they will not go back to where they want(their initial app- LinkedIn) but back to Bookmark activity.</p>
            <img width="918" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/5b85e44c-f532-41c9-a1f0-ea1bfa829589">
           * **Single Instance** launchmode will also launch a different task independent of the previous active taks but the difference is this new Browser activity which was opened is completely isolated so inside it you are not allowed to open any other activities (payment app paypal)and the user cannot interfere with other apps while on it(security risk)</p>
 
      - [x] [ViewModels & Configuration Changes](https://www.youtube.com/watch?v=9sqvBydNJSg&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=5)
            <details><summary>Summary</summary>
           * **MVVM**
           * 1. Generally, the View Model's job is to take the raw data from Model and bring it into a new format easy to display in the UI.The View Model will convert data from Model -> into a format that UI understands and as soon as that happens the View Model will then automatically notify the UI that there is a change so that the UI can update and show new info. Whenever something has to do with Real Data Source(DB) VM sends new data to Model the Model saves it and notifies the UI again. 
           * 2. No Model! - VM has the responsibility to chage the state and notify UI - When user clicks to change bakground colour we call VM. (UI -> sends UserAction to ViewModel so the VM can react to it) that doesn't need the Model since the UI action would be the button click, the VM updates the state that the background colour changed and notifies the UI so the UI can show the background colour. VM receives a User Action/UI Action/Event from the UI(View) -Button Click,Swipe different page
          <img width="1124" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/d2b5ad36-dc14-49e7-b024-759aa24fbfe6">
          * Configuration change - screen rotation, user changes language, theme - app needs to update all colours.How Android deals with these changes is by re-creating the whole activity(current instace of activity distroyed- lifecycle moves to onDestroyed state and when the rotation finished it will start with a new activity). The VM will also be re-created.
          * Eg below where on screen rotation the background is not changed </p>
           <img width="573" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/9f59460e-a900-4679-820a-0609d9ab8507">
           <img width="573" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/7169cd75-3396-4d04-9338-61e40bf35951">
          * Eg below where on screen rotation the background is changed
          * Inheriting from ViewModel it will create a component which will outlive the life cycle of its screen(activity). The activity has a lifecycle that ends when we rotated the device then this VM that it inherits from will outlive and won't be distroyed when the activity will be distroye. It will be distroyed when use pops the activity from the backstack(back button)</p>
          <img width="573" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/eb1a8034-97cf-4462-921b-5684a5095101">
          * The VM won't be destroyed because of configuration changes we need to use the Android way of initialising the View Models</p>
           <img width="738" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/6ed0c59f-deb4-4035-9d66-d70e12f83ae7">
          * View Model factory - a class that defines how our viewModel instance is to created with the Android ViewModel</p>
          <img width="800" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/6660238b-6370-4ee6-abaf-e73444e0ae5e">
     
     - [x] [What is context?](https://www.youtube.com/watch?v=YdnM2ZvrIFM&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=4)
        <details>
         <summary>Summary</summary>
         
         * Context is a super class. Context object comes from Android Content.
         * It's brigde between YOUR Android app and the rest of Android Operating system.
         * It provides **context** for your app to operate within the larger scope of whole Android Operating System.
         * Your app needs to communicate to other system/components or other apps(eg get access to resources- static images, localised strings you need access to context) another eg(DB or preferences). To get these you need access to the context.
         * Where DB needs to save something on your Android device & because that file system is an Android component(part of Android system) you need context to write to this file system)
         * If you want to launch a different Activity from your app or from another - you need Context in order for your app to read a text file in an app that supports text files - to open that other Activity which is able to read the textfiles that would need Context. It's the middle man between your app and other components.
         <img width="547" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/cbfcc242-17dd-42f5-9e35-067fa4b70c36">
         * A kotlin class doesn't know how to interact with my Android app, where to save data etc, so it needs access to a context object. Now it's connected to the Android side. and can use this context intance to do all of these things: write to files, open DB connections.
       <img width="547" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/2c0ac4d0-7250-4d67-9801-baec0e54e412">
         
         * Context is a Superclass. It's s how your android app interacts/gets access to other components/apps.
         * Subclasses of Context:
             - Activity Context (Main Activity)
             - Application Context (MyApplication - Different Application)
             - Services etc
         <img width="516" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/9bf8fa62-9466-49a8-b862-aabbee223afc">
         
         *  What's the difference between a Application Context(MyApplication class) and an Activity Context(Main Activity)?
         *  Each context has a specific lifetime.
         * Activity context is active as long as the activity is active, each activity has a lifecycle - and when Activity is destroyed all it's components are destroyed and resources freed up, including Context.
         * When App(My application) is destroyed - Context is destroyed also.
         * Conclusion
         * Context is "the gateway to Android services" - this means connects with other apps in terms of permissions(if has permission connects if not then NO!) "and application storage" - Each context has a specific lifetime.  When MainActivity is destroyed all it's components are destroyed and resources freed up, including Context. When App(My application, an API) is destroyed - Context is destroyed also.
         * What we want is not to store activity context outside of activity. Eg setting a view Model's context to have the same lifecycle as the main activity because it will outlive the lifecycle of the activity.
         * _Basically we don't want anything to outlive our MainActivity._ "E.g.When thelifecycle of the View Model is longer than the Activity (View Model had an instance of the activity) this could mean memory leaks.
          <img width="968" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/87b0b736-9214-43cd-b7fc-4f11739003d1">
          
          *  Do we benefit from having different context lifetimes? Yes, they can lead to memory leaks. Don't store activity context outside of an activity at least not in components who have a different lifetime. Eg setting a view Model's context to have the same lifecycle as the main activity.The VM's lifecycle will outlive the lifecycle of the activity
           <img width="968" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/1440ffc5-a5ee-4150-8a69-ecd6f2a3b948">

          * Why do we need Activity Context?
          * When you need information about the activity itself. you want to request certain premissions when you want to access private user info or using the phone's camera, microphone. You need to request the permission from the user to access that.
          * `ActivityCompat.requestPermissions(pass in activity context and not application context)`
          * `requestPermissions()` shows a system dialogue(overlay a transparent activity that comes from the Android system but this activity needs info about your current activity because it will show on top of it). This is connected to your UI if you want to see the permission dialogue. The App Context is not connected to the UI because that just refers to the App itself and your app could just be in the background if you access your application context. 
          * <img width="466" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/f5042da9-17c7-4123-b059-7a4161d8b1a2">
        </details>
  
      - [x] [Resources and Qualifiers](https://www.youtube.com/watch?v=vj1ZdUfPlJM&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=5)
        <details>
         <summary>Summary</summary>
          
         * Resources are non code things you app needs: Pictures, Vector graphics, localised Strings(text translated to different languages so your app can support that as well). `res` folder
         * `drawable` relates to everything visual - pictures,jpeg, vector graphics(translated in XML format)- SVG image then you can import it here and Android Studio will convert it into an XML format which Android understands. 
          <img width="222" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/897dc548-59a5-4c4e-bea1-7807615d9c4e">

         * Copy-Paste the picture into drawable

         * Now we want to read the picture and get a reference to it in code.
         * Every resource has an ID (R - your package name)
         * For Applications use `applicationContext.resources`
         * For our Activity we use `resources.getDrawable(R.drawable.anime)`
         * If you want to show it on the screen directly
        <img width="951" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/cf97d1ee-90b8-403f-9c3a-750610361d4d">

         * `drawable` we have ic_launcher of same type (v24) is a qualifier - this is used for a specific device configuration - that means that Android device neds to run @least on API level24 otherwise this resource won't be used. Eg some devices where apps only available for that Country code,  Small screen width , one resource only on dark mode
           <img width="251" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/56287a6a-6771-4f4d-b9c8-77df0258f59a">
           <img width="624" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/2bbdfa65-8214-481f-afeb-7b2762e866d5">
           * `Mipmap`  is used for the Icon of our app  - no matter size or resolution of screen,Lots of qualifiers mdpi,xhdpi that refer to the device resolution - better resolution the higher we go xxxdpi is the higher
             <img width="277" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/229c4123-fc8c-48b1-8cb2-9efbe1c4c71a">
             
           * Vector graphics - still in drawable - if you want some images to just be in night mode.
           * Drawable> New> Drawable New Resource file> Select NightMode
           * Qualifiers(Night Mode) - configuration that we make our resources dependent on.
           * Copy and paste the night mode image into drawable int a new directory called `drawable-night` and move in Project view. Go to night mode and you will see it change.
            <img width="318" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/05e64dcb-d7a6-4468-973b-e096070511a4">

           * Values combines colours, strings and themes
           * Add a New Values Resource > call it colors > select Qualifier > Night Mode &replace the colours for night mode. 
             <img width="796" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/e9a15289-4edb-416c-89dd-9ba7f4820126">
             <img width="277" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/458be670-fa15-40e9-8eac-a16312cf2c55">
      
            * Strings - New Value Resource > Locale>Choose a country
            * Themes  - define themes directly in compose, so not used
            * xml - config for specifics that don't fit above
            * Conclusion - you can access any recource if you have access to the activity or context of the app referring to resources - applicationContext.resources. 
         </details>
         
      - [x] [Intent & Intent Filters](https://www.youtube.com/watch?v=2hIY1xuImuQ&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=6)
            <details>
              <summary>Summary</summary>
          * Intent is a way to communicate with a different android component(an activity). Like an envelope that holds the intention of your app and transfers that to a diff android component(usually an activity).
          1. Explicit Intent tageted towards one specific app that has to be specified in that intent - we speficy the intention "we want to launch that youtube app and when we fire and send that intent Android will launch that youtube activity."
          * _We explicitly mention an Action (a thing we want to do with that intent) because it's only sent to one specific app... either to our app or other(Youtube)_
             * 1. Example of Explicit Intent
               * Create -a Second Activity to our Main app and register it in the `Android Manifest`.
               *  `Android Manifest` = the place that summarisez the functionality of your App. Shows to the outside world "This is what your app needs to do and these are:

                  - the Components it consists of
                  - the Permission it needs "  - to access the User's camera that needs to be registered.
            <img width="635" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/154f5a84-6278-422e-a137-73963ad839ec">
            
              * When we Click the Button in the Main Activity -> We want to create an **Intent** with the intention to launch the Second Activity and then fire that and actually Launch it. We link it to package context(the context of our app) & class overload(class of our second activity)
                
              `Button(onClick = {
                       Intent(applicationContext,SecondActivity::class.java)
                   }`
              `.also{startActivity(it)}` requires an intent object - it(Intent above) Run app and you will get to second screen.
            <img width="1426" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/9d7a67df-f41e-47e5-96ca-90155d7438e3">
            <img width="249" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/b5e332de-0c4d-48ef-911e-9035974263db"> <img width="249" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/bf026b28-1a67-430d-8fe8-ee870bbe9b19">
        
           
           * 2. Another Example of Explicit Intent
              
              * Open another App from Package Manager and not the one we built - To Lanch an App that is installed in the device we need it's package name(Youtube)
              * We pass an Action
              <img width="432" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/a8284b23-ca52-4ef2-bbb6-294b5bbedbc1">

                `Intent(Intent.ACTION_MAIN).also { it.`package`= "com.google.android.youtube"
                
                           try {
                               startActivity(it)
                           }catch(e:ActivityNotFoundException){
                               e.printStackTrace() // if we can't find the Activity print the stack trace
                           }
                       }`
              2. **Implicit Intent** just specifies an action(smth you want to do with that intent) and Android will check which apps can actually satisfy that intent and show the user a chooser, so they can choose which app they want to send that intent to or open.
                 
             * Eg. If you want to open a text file in your app but your app can't do that because you don't have that code. You want to send the user to a different app that can open a text file but you don't care whcih app that is, you just want that app that can open a text file. You want to send an email (you  won't implement the code for that ) you would rather open an email app (Gmail) and pass all that info to that intent so that Gmail can handle that.

             * `Button(onClick = {
               
                        val intent = Intent(Intent.ACTION_SEND).apply {` --> Action_send = send email
               
                             type = "text/plain"  --> specify the type of data to send image, text
                             putExtra(Intent.EXTRA_EMAIL, arrayOf("test@test.com"))
                             putExtra(Intent.EXTRA_SUBJECT, arrayOf("This is my subject")) --> subject of email
                             putExtra(Intent.EXTRA_TEXT, arrayOf("This is the content of my email"))} --> email content
               
                         if(intent.resolveActivity(packageManager) !=null) { //check to see if there are any apps that satisfy these requirements
                            startActivity(intent)}
             
             *`Manifest`
             * `<queries>
                   <intent>
                   <action android:name="android.intent.action.SEND"/>
                   <data android:mimeType="text/plain"></data>
                    </intent>
                </queries>`
               <img width="257" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/cc4d3eab-d6b5-44d7-beaa-c61ba526e95b">
               <img width="246" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/285d77e4-ea5a-4fa2-bb6a-9d34b89d440f">
               
             3.  If you want to register your app to **receive an Intent**
                  * Your app can pop up in a App Chooser where other apps can see by using an Intent Filter
                  * Intent Filter - we can specify that our app receives tabs of intents
                  * Share image - Chrome will send an intent that it wants to share an image.
                  * If you press More - that will now show all apps that can accept such images.
                  * Set up your app to receive an image and show that image in our app > Manifest> specify intent filter
                  * Register the intent in the Manifest
                    <img width="514" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/70bc23c3-e567-452e-801a-691c76ea7138">
                    <img width="222" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/9744b9c1-d239-4e13-ab17-0396cad55504">
                  * But you won't see the Image when you are sharing in the More(Package Manager).We haven't received that intent yet from Chrome App.
                  * Chrome needs to put that data of the image inside that intent which then is being sent to our app. But our App needs to have the power to show that image, and by default what Chrome(that intent) will do is launch a new Task of our App (a new instance of our app) whcih will get that intent onCreate if you wanted or
                  * Add in Manifest in Launchmode- if there's an instance of the app already open just send the data to that active instance. Setting the launchmode to Single Top. Manifest -->  android:launchMode="singleTop"
                   * It will trigger `override fun onNewIntent(intent: Intent?) {super.onNewIntent(intent)}` because there's not a new Activity that is created so onCreate wouln't be called again but this `onNewIntent()` will be called and will deliver this intent from Chrome
                   * so you can get the `uri` - the address of that image on our device which you ca read in as a byte.
                   * `var uri =intent?.getParcelableExtra(Intent.EXTRA_STREAM, Uri:: class.java)`
                   * `getParcelableExtra()` - package or serialize some data
                   *  surround with a version check <img width="750" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/f30cf4c8-4da7-460c-904c-14695a3b9624">
                   * we want to take the uri and display it in an image that we can put in UI
                   * create a simple view model - that will update the state of our composables
                   <img width="750" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/3171acb8-0367-46af-8ff3-06d8d70cc0bf">
                   * create an instance of viewModel
                     <img width="503" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/a543a2f1-12c3-41c9-8128-d5822da8ea1f">
                     * and submit that uri
                       <img width="199" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/fa263e8e-b416-457c-88c0-60baffe5b67b">
                     * Go in Gridle Scripts module app to add a image loader, image caching library ` implementation("io.coil - kt:coil-compose:2.4.0")` uri to byte process it too complicated so we use this
                     * ![image](https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/4b38ef44-196a-44c5-b024-58d1251e3e75)

                     * Go into Google -> go into an image -> Share Image -> More -> Select your app -> the image will show in your app
            </details>
            
      - [x] [Broadcast and Broadcast Receivers](https://www.youtube.com/watch?v=HDVyFsFUuVg&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=7)
            <details><summary>Summary</summary>
           * Broadcasts are system-wide evets your app can consume and receive.
           * Sending a boradcast(like an intent) to many apps and apps that receive a broadcast.
           ***Registering for Broadcast:**  Your app can register a broadcast receiver which is triggered when a roadcast is received
           * Eg: when the Android device is booting up. Android system will send a broadcast to all apps
            that are registered to receive this specific boot broadcast so that the apps can react when the device is booted up.
           * Eg.2 Listening to music and getting a call. Phone calling app sends a broadcast so other apps can react to it. Music player could pause the playback so that user can fully accept the call.
           * Eg 3. Airplane mode - When the user toggles off airplane mode we want to react to that and also turns back on.
           * Broadcast receiver is a class
             <img width="560" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/d88c6a09-2ea3-4171-b6c4-aaf9ecf93ec8">
           * Register the Receiver and specify an intent filter 
             onCreate() you register the receiver specify intent filter((what kind of intents our receiver should receive). Intent filter - pass the action of the intent to be received-Intent.ACTION_AIRPLANE_MODE_CHANGED
          * Unregister this airplane mode receiver when it's not needed anymore - In the case of an Activity that would be onDestroy
          * Dynamic broadcast receiver - dynamically declare when we need it (eg. in registerReceiver-airplaneModeReceiver function) and we dynamically unregister it onDestroy
          * This will only work if our app is active,
             `private val  airPlaneModeReceiver = AirPlaneModeReceiver()`
            
             `override fun onCreate(savedInstanceState: Bundle?) {
                super.onCreate(savedInstanceState)
                registerReceiver(airPlaneModeReceiver,IntentFilter(Intent.ACTION_AIRPLANE_MODE_CHANGED)`
            
             `override fun onDestroy() {
                super.onDestroy()
                unregisterReceiver(airPlaneModeReceiver)`
            * Toggle the Airplane mode on and check Logcat for the printline
            * <img width="560" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/48023a49-f357-48eb-a6ed-86cf2a90ee68">
            </details>
            
        - [x] [Foregroud Services](https://www.youtube.com/watch?v=YZL-_XJSClc&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=8)
        - [ ] [Work Manager](https://www.youtube.com/watch?v=A2JetouoNSc&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=9)
        - [ ] [URIs - Unique Source Identifier](https://www.youtube.com/watch?v=4Ob0plBL084&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=10)
        - [ ] [Content Providers](https://www.youtube.com/watch?v=IVHZpTyVOxU&list=PLQkwcJG4YTCSVDhww92llY3CAnc_vUhsm&index=12)


3. - [ ]  [Modern Android App Arhitecture](https://developer.android.com/courses/pathways/android-architecture) Mentor advice
4. - [ ]  [Guide to App Arhitecture](https://developer.android.com/topic/architecture) Mentor Advice
   - [ ]  Android framework [Platform arhitecture](https://developer.android.com/guide/platform)
       
   - [ ] [Android Fundamentals for Beginners](https://www.youtube.com/playlist?list=PLQkwcJG4YTCTq1raTb5iMuxnEB06J1VHX)
   - [ ] [Gradle for Beginners](https://www.youtube.com/watch?v=o0M4f5djJTQ)
   - [ ] [Convert Figma Designs to Jetpack Compose Code With This FREE Plugin](https://www.youtube.com/watch?v=byOmrmXG4yQ)

  - [x] [Text Fields - UX With Material3](https://www.youtube.com/watch?v=ZERIxmBYP-U)
  - [x] [Custom Layouts In Jetpack Compose - Crash Course](https://www.youtube.com/watch?v=bTgyDqBoZ_o)
   - [ ] [Custom layouts and graphics in Compose](https://www.youtube.com/watch?v=xcfEQO0k_gU)
   - [x] [Brush: Gradients and Shaders](https://developer.android.com/jetpack/compose/graphics/draw/brush)
      - [x] [Apply Hex Color Code to your Jetpack Compose Project Easily](https://www.youtube.com/watch?v=zlqXzE0al5s)
      - [x] [Gradient Button - Jetpack Compose](https://www.youtube.com/watch?v=vPOS6L2SEX0)

   - [ ] Screen reader https://www.w3.org/WAI/standards-guidelines/
   - [ ] https://chrome.google.com/webstore/detail/headingsmap/flbjommegcjonpdmenkdiocclhjacmbi
   - [ ] https://www.nvaccess.org/download/
   - [ ] https://dequeuniversity.com/screenreaders/nvda-keyboard-shortcuts
   - [ ] Testing explanation: https://www.google.com/imgres?imgurl=https://i0.wp.com/4.bp.blogspot.com/-lgR0Ph-CLnE/UZ9CJXaaRlI/AAAAAAAAAyY/D0zkoc3KnVA/s1600/TestingTriangle.png&tbnid=b8wvWS1MlDn44M&vet=1&imgrefurl=https://www.allankelly.net/archives/628/testing-triangles-pyramids-and-circles/&docid=30gYx_begKiw-M&w=1600&h=1363&source=sh/x/im/1

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

Arhitecture - https://developer.android.com/topic/architecture/intro

#### Testing:
- [ ] Testing in Android [****](https://www.youtube.com/playlist?list=PLQkwcJG4YTCSYJ13G4kVIJ10X5zisB2Lq)
- [ ] https://developer.android.com/jetpack/compose/testing-cheatsheet
- [ ] https://developer.android.com/jetpack/compose/testing
- [ ] https://developer.android.com/codelabs/jetpack-compose-testing?authuser=1#1
- [ ] https://youtu.be/kdwofTaEHrs


# Kotlin
#### Android Kotlin courses
  <details><summary>Summary</summary>
  
- [ ] [Kotlin from newbie to pro](https://www.youtube.com/playlist?list=PLQkwcJG4YTCRSQikwhtoApYs9ij_Hc5Z9)
- [ ] https://developer.android.com/courses/android-basics-kotlin/course
- [ ] https://developer.android.com/kotlin
- [ ] KOTLIN NEWBIE TO PRO https://www.youtube.com/playlist?list=PLQkwcJG4YTCRSQikwhtoApYs9ij_Hc5Z9

- [ ] [Kotlin Enums](https://www.youtube.com/watch?v=1rW52kazuJk)
        <details><summary>Summary</summary>
        <img width="609" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/06388671-62a6-428c-8a1f-bcbc084bbfc4">
        <img width="609" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/353c70c2-93f6-4585-8658-0d137613f8ce">
        <img width="782" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/420a302e-0f0a-4bc1-a98d-2ab519fffeef">
        <img width="998" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/b0267802-87b2-48e4-8586-12cb73f7444a">
        you add in the parameters to the enum class to be able to access the values you pass in.
        <img width="924" alt="image" src="https://github.com/lauravoineag/MobileAndroidDeveloper/assets/77536595/d7ebe262-f6f7-4936-9a8e-f07be1fc4cf9">
        </details>
</details>

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

# 4. Other platforms for learning Language:
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


Adding on the pile 
[Android how to start](https://developer.android.com/courses)
[Android Development with Kotlin](https://developer.android.com/courses/android-development-with-kotlin/course)
Good to know:

https://developer.android.com/studio

[Key Promoter](https://plugins.jetbrains.com/plugin/9792-key-promoter-x/versions/stable)

Interview prep:
https://www.youtube.com/shorts/VLdPutYuxrw
