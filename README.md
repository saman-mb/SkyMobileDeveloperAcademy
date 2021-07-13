
# Movie Trailers Mobile App Exercise

![](https://www.latestfreestuff.co.uk/wp-content/uploads/2017/04/Free-Sky-Movie-Worth-£13.99.png)

## Brief

Sky would like you to build movie trailers app that presents information about movies from an API in a list and also allows users to select more details about a particular movie!

### Requirements

- User interfaces for two distinct screens should be implemented
- The first screen will show a list of movies to the user
- The second screen will show the details about a particular movie to the user
- Tapping a movie from the list should present that movies details to the user
- On both screens the user should see a loading spinner when the screen is loading the data
- If the data fails to load for some reason the user should see an error message

#### Bonus Requirent!

Allow users to play the trailer for a movie from the programme details page.
- The user should see a play icon on top of the programmes image
- Tapping the play icon should begin playing the movies trailer

### API Details

[Movies list API:](https://saman-mb.github.io/SkyMobileDeveloperAcademy/movies.json)

[Movie detials API:](https://saman-mb.github.io/SkyMobileDeveloperAcademy/movies/{uuid}.json)

### Resources 

Play Icon Image: https://saman-mb.github.io/SkyMobileDeveloperAcademy/resources/play.jpg

### Docs

Android Developer Ref: https://developer.android.com/docs
Build your first app: https://developer.android.com/training/basics/firstapp
Android basics in Kotlin: https://developer.android.com/courses/android-basics-kotlin/course
Kotlin Docs: https://kotlinlang.org/docs/home.html
Introduction to Android Activities: https://developer.android.com/guide/components/activities/intro-activities
Android Media Player Docs: https://developer.android.com/guide/topics/media/mediaplayer


## User Story

#### AC1
- Given I launch the movie trailers app
- When the movies data is loading
- Then I should see a loading spinner
- When the movies data finishes loading successfully
- Then I should see a list of movies *(see note for more info)*

**Note:** *Each item in the list should show the movies title, image, and parental rating*

#### AC2
- Given I launch the movie trailers app
- When the movies data is loading
- Then I should see a loading spinner
- When the movies data fails to load
- Then I should see an error message explaining that something went wrong *(see note for more info)*

**Message text:** *"Oops, something went wrong. Please check your connection and try again."*

#### AC3
- Given I am currently looking at the movies list
- When I tap on a movie
- Then a new movie details page should be presented to me
- When the movie details data is loading
- Then I should see a loading spinner
- When the movie details data finishes loading successfully
- Then I should see more details about that movie I selected

**Note:** *The movie detail screen should show the movies title, image, rating, and synopsis*

#### AC4
- Given I am currently looking at the movies list
- When I tap on a movie
- Then a new movie details page should be presented to me
- When the movie details data is loading
- Then I should see a loading spinner
- When the movie details data fails to load
- Then I should be taken back to the facts list
- And I should see a standard system alert containing a message explaining that something went wrong

**Alert title text:** *"Oops, we could not load that movie."*
**Alert body text:** *Please check your network connection and try again.*

#### AC5 Bonus!
- Given I am currently looking at a movie details page
- When the movie has a trailer available
- Then I should see a play icon displayed over the top of the image
- When I tap the play icon
- Then I should see the movie trailer video playing full screen

**Note:** *The play icon image file is listed in the resources section above in this doc.*
**Note:** *Mobile platforms offer a native video player which can utilise the playback urls provided in the API response, please look at the docs linked in the resources above for more info on this.*
