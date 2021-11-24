The application uses the Google Calendar API to fetch upcoming events


## FEATURE 2: SHOW/HIDE AN EVENT’S DETAILS
### User Story: As a user, I should be able to toggle an event’s details, so that I can expand or collapse the information as needed.
Scenario 1: An event element is collapsed by default.
Given the user is searching for an city
When the user has selected a city
When the user clicks the collapse button
Then the event element should collapse

Scenario 2: User can expand an event to see its details.
Given the user has an event open
When the user clicks on the event
Then the user should see the details of the event

Scenario 3: User can collapse an event to hide its details.
Given user is looking at the details of an event
When the user clicks the collapse button
Then the event element should collapse




## FEATURE 3: SPECIFY NUMBER OF EVENTS
### User Story: As a user, I should be able to specify number of events, so that I can control how many events are displayed per city view
Scenario 1: When user hasn’t specified a number, 32 is the default number.
Given user has a city selected
When the user does not specify a number of events to show
Given user has a city selected
When the use specifies the number of events shown
Then that number will be the max number of events shown

Scenario 2: User can change the number of events they want to see.
Given user has a city selected
When the use specifies the number of events shown
Then that number will be the max number of events shown



## FEATURE 4: USE THE APP WHEN OFFLINE
### User Story: As a user, I should be able to use the app when offline so that I can still get event information without an internet connection
Scenario 1: Show cached data when there’s no internet connection.
Given the user has no internet connection
When the user runs the app
Given the user has no internet connection
When the user tries to change settings
Then an error message should show on the screen and the change should be prevented

Scenario 2: Show error when user changes the settings (city, time range).
Given the user has no internet connection
When the user tries to change settings
Then an error message should show on the screen and the change should be prevented


## FEATURE 5: DATA VISUALIZATION
### User Story: As a user, I should be able to see a visualization of event numbers, so that I know how many upcoming events are in each city
Scenario 1: Show a chart with the number of upcoming events in each city.
Given user is on the main page of the app
When the user wants to look at the number of events in multiple cities
Then a chart showing the cities and number of events per city is shown
