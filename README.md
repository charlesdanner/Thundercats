# Next Game

A group collaboration during the UNCC Programming Boot Camp. This application is the group's best attempt during the allotted time the assignment was tasked to create their own website. We wanted to create an application that would help people who play video games find a new game to play. Based on user input we access either the IGDB API or Rawg.io's API to find games that are similar to the titles that the user inputs or for the specific game they input. The site uses local storage and a firebase user authentication system for enhanced user experience. Users can keep track of their search history, games they're interested in and different stats that are kept track of and updated throughout their use of the site. 

## Prerequisites

In order to use the site users must sign up using one of the buttons in the site's nav bar. A basic form will ask for their email and password. 

## Under the Hood

The page uses a firebase authentication function. The contents of the page are initially hidden until the authentication change listener gets triggered. When this happens it reads whether the user is signing in or signing out. If signing in, the nav bar is manipulated and the contents of the page are shown using Java Script. If signing out, the contents are hidden and the nav bar is again manipulated so that the only buttons that are usable are for users to either sign in or sign up. This makes it so the website is locked behind a sign in process. The main purpose of the site, finding games and information about them, is done using two separate APIs. Rawg.io and IGDB, specifically. These are both done through AJAX calls in Java Script. When the similar games radio is selected when users select 'search for games' the data is being parsed through using Java Script. The cover and title are both stored in memory in divs and appended as a list item. From there the list item is appended to the carousel made using the UI Kit framework. Clicking on the games makes another API call to IGDB's API and the game title and information are appended into a modal that pops up. The wish list and search history are both stored in arrays that are commited to local storage whenever they get updated throughout the user's use of the site. Users can delete individual items in these fields by clicking the 'x'. Java Script uses the splice function to do this.

### Built With
* BootStrap
* UI Kit
* Java Script
* JQUERY
* Rawg.io
* IGDB

### Authors
* Charles Danner  https://github.com/charlesdanner
* Shawn Galloway https://github.com/shawngway
* Tim Cockerill https://github.com/dtimcockerill2
* Zion Brown https://github.com/LardianGH
* Anthony McPherson https://github.com/aqm28202

### Link to live site: 
https://shawngway.github.io/Thundercats/
