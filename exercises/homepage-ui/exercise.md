# Homepage Rails UI Exercise

## Brief

Implement a rails based home page UI for your elected mobile platform (Android or iOS) that scales correctly on both tablet and mobile devices. 

The UI should support the following rail template types 
`[hero, wide, cover, square]`

The entire page should be scrollable both vertically and horizontally within each rail component. *Examples in other apps:* _Sky Go, Netflix_ 

## Overview 

1. Make an HTTP GET request to [https://saman-mb.github.io/SkyMobileDeveloperAcademy/exercises/homepage-ui/resources/homepage-ui.json](https://saman-mb.github.io/SkyMobileDeveloperAcademy/exercises/homepage-ui/resources/homepage-ui.json)

2. Parse the data in the response to a Swift struct or Kotlin data class. 

3. Use the parsed object representation of the json as the source of truth for rendering the homepage UI. 

### Hints: 
- _The json file represents the data we want to present in the page and is also structured hierarchically in a that maps in a 1:1 relationship to the structure of the UI. _

- _dont worry about making the sizes and spaces exact, only try to pick values which approximates the wireframes_

-  _you may notice that some of the properties in the json response are optional, try to think about how to handle the absence of the these values in your code_

- _phones have less screen real estate than tablets so try to think how to build your UI so that we can maximise the space depending on which device were running on. How can we scale down the size of the cells for mobile without changing their aspect ratio?_ 


## UI Wireframes 

<img src="./resources/cell-types.png" width="400"/>

<img src="./resources/phone.png" width="500"/>

<img src="./resources/tablet.png" width="800"/>
