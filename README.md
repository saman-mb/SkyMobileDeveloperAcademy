<img src="https://user-images.githubusercontent.com/52349/136939032-ae5ad45b-fbd0-4f8f-8631-50eba7c85743.png" alt="drawing" width="200"/>

# Mobile Academy 
## Sky Go Training Project 
### App Brief
* Build an OTT VOD browsing and steaming app that uses native DRM protection. 
* Native Android and iOS App 
* Share code via a GraphQL service intially running on local host but later can be deployed somewhere
* Target architecure MVVM or MVP 
* Potentially build UI using latest APIs (Swift UI / Jetpack Compose)

### Stories
* App Startup / Splash Screen 
* Home Page  
* Show Page 
* Login Page
* Play VOD
* Settings 

### Tech Tasks
* Analytics / Logging 
* CI 
* Unit Testing 
* Testing 

### Splash Screen / App Startup 

Build an animated splash screen page which stays displayed until the app has finished carrying out the necessary startup processes before transitioning to the home page. 

* *On app launch* - show splash 
	* hit [init.sky.com](init.sky.com) - persist country code / server time offset 
	* hit [config.sky.com](config.sky.com) - persist config 
* *On app foreground* - show homepage 
	* hit [init.sky.com](init.sky.com) - persist country code / server time offset 
	* hit [config.sky.com](config.sky.com) - persist config 
* *On error* - show startup error 
* *On success* - load the home page 
* Handle application life cycle events 

### Home Page

Build the page that presents VOD content to the user to browse after the app finishes loading. 

* Hit QMS or a hosted json file defining some rails with different render hints 
* For each rail make a w2w call 
* Loading spinner 
* Show the content 
* Build the UI components and plug it all together 

### Show Page 

Build a page which presents metadata for single and episodic programmes to the user in a modal context. 

* present the show page with loading spinner 
* make a W2W call 
* render the page meta data 

### Login Page
* Rango integration 
* Native UI 
* Persist the oath token to disk securely 

### Play VOD 

Build a video player which is capable of playing both unencrypted and encrypted Sky VOD assets using Native DRM. (FairPlay, Widevine)

* If user isn’t logged in show login 
* Initial version can use unencrypted test stream
* Final version can use OVP integration and native DRM (FairPlay, iOS / WideVine, Android) 
* Build the video player UI 
* Local bookmarks 

### Settings 

Build a page that displays useful app information and settings to the user in a modal context. 

* Terms and conditions page 
* Player settings 
* Persisting users selections across app sessions 

### Analytics 

Build a logging system that allows developers and analysts to debug problems as extract useful information about how customers are using the app. 

* Build generic modular logger (or use an off the shelf solution to keep things more simple)
* Log levels 
* Device log 
* Third parties: Firebase, Sentry, Adobe (needs some discussion as we want to keep things simple)
* Crash reporting 

### Testing
* testing pyramid 
* unit testing 
* ui testing 

### CI 
* Set-up a simple build and test pipeline in Jenkins 
