# Homepage Rails UI
## Exercise

Implement a rails based home page UI for your elected mobile platform (Android or iOS) which scales and renders correctly on both tablet and mobile devices. 

### Overview 
1. make an HTTP GET request to https://saman-mb.github.io/SkyMobileDeveloperAcademy/exercises/homepage-ui/resources/exercise.json

2. The json file represents the date we want to present in the page and is also structured heirachichally in a way that maps 1:1 with the structure of the UI. Parse the data in the response to a Swift struct or Kotlin data class. 

3. Use the parsed object representation of the json as the source of truth for rendering the homepage UI. 

### Hints:
- dont worry about making the sizes and spaces exact, you can pick your own values which aproximates the wireframes 

-  you will notice that some of the properties in the json response are optional, try to think about how to handle the absence of the these values in your code  

- phones have less scren real estate than tablets so try to think how to build your UI so that we can maximise the space depending on whih device were running on. How can we scale down the size of the cells for mobile without changing their aspect ratio? 


### UI Wireframes 

<img src="./resources/cell-types.png" width="400"/>

<img src="./resources/phone.png" width="500"/>

<img src="./resources/tablet.png" width="800"/>