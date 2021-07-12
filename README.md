
# Movie Trailers Mobile App Exercise

![](https://www.latestfreestuff.co.uk/wp-content/uploads/2017/04/Free-Sky-Movie-Worth-£13.99.png)

## Brief

We would like you to build movie video player app that presents movie information from an API in a list format and allows the user to select a fact to present more details to the user. The first screen will show a list of facts to the user. When selecting a fact a second screen is presented to the user showing more details about that fact. We also want to see some indication when the data is loading as well as messaging to handling any potential errors that may arise.

### Requirements

- The app should be written in Swift. You can use the latest tooling / swift version if you like, or something a little older it's not all that important.

- Please do not import external dependencies such a networking libraries, futures/promises libraries or reactive libraries. We are more interested to see how you approach solving the exercise using just the vanilla Apple SDKs.

- It is up to you to decide how the UI looks, what is important for this exercise is that all the ACs are met precisely and that the application works as per the requirements.


### API Details

**Movies list API:**

`https://saman-mb.github.io/SkyMobileDeveloperAcademy/movies.json`

**Movie detials API:**

`https://saman-mb.github.io/SkyMobileDeveloperAcademy/movies/{uuid}.json`

<div style="page-break-after: always;"></div>

## User Story

###AC1
- Given I launch the cat facts app
- When the facts data is loading
- Then I should see an in page loading indicator
- When the facts data finishes loading successfully
- Then I should see a list of cat facts

**Note:** *each item in the list should show the fact as well as the number of upvotes*

###AC2
- Given I launch the cat facts app
- When the facts data is loading
- Then I should see an in page loading indicator
- When the facts data fails to load
- Then I should see an in page message explaining that something went wrong

**Message text:** *"Something went wrong. Please check your network connection and try again."*

###AC3
- Given I am currently looking at the cat facts list
- When I tap on a fact
- Then a new page should be presented to me modally
- When the fact details data is loading
- Then I should see an in page loading indicator
- When if the fact details data finishes loading successfully
- Then I should see more details about the fact I selected

**Note:** *The detail screen should show everything about the fact select shown on the list page as well as whether or not the fact is verified and the date the fact was last updated*

**Example verified messages:** *Verified / Not Verified*

**Example Date message:** *2 October 2020, 10:26*

<div style="page-break-after: always;"></div>

###AC4
- Given I am currently looking at the cat facts list
- When I tap on a fact
- Then a new page should be presented to me modally
- When the fact details data is loading
- Then I should see an in page loading indicator
- When the fact details data fails to load
- Then I should be taken back to the facts list
- And I should see an alert containing a message explaining that something went wrong

**Alert title text:** *"We could not load the details for that fact."*

**Alert body text:** *Please check your network connection and try again.*
