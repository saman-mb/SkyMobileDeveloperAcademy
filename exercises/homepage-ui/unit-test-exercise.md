# Homepage Rails UI - Unit Tests Exercise

## Brief

So you have now built a rails UI by integrating with a back end service, parsing the response, mapping the response to a domain model type and then using that model to configure the view. 

Now let’s consider improving the code to follow a clean architecture approach that should also make things easier to unit test! 

I have created a swift playground to outline the basic structure of making the homepage conform to MVVM. At the bottom I have put some example test functions to help get you thinking about which sorts of things we should be testing at each layer in the architecture we’re using. 

### iOS App

1. refactor your code to follow the MVVM architecture
2. use the `XCTest` framework to unit test your model and view model
3. implement your own mock objects by using protocols


#### Docs
https://www.hackingwithswift.com/read/39/2/creating-our-first-unit-test-using-xctest
https://www.swiftbysundell.com/articles/mocking-in-swift/

### Android App

1. refactor your code to follow the MVVM architecture  
2. use the `JUnit` library to unit test your model and presenter
3. use a mocking framework like `Mokito` to mock 

#### Docs
https://kotlinlang.org/docs/jvm-test-using-junit.html
https://developer.android.com/training/testing/unit-testing/local-unit-tests
https://site.mockito.org
