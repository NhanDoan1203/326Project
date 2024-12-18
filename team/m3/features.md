# Application Features

## Feature: TrailSafe Insights

This feature retrieves trail data on the hikers previous saved trails using indexedDB. It uses this data 
to create a visualization dashboard that shows insights to the hiker. This is used to give the hiker data on such as 
total mileage hiked, longest hike, and total hikes. This feature is fully integrated with the TrailLogService
to utilize indexDB for persistence. 
**Point Value**: 4 
**Completed By**: Blake Thomas

## Feature: TrailLogService

This feature uses IndexedDB to create a service to log trail data to preserve hiker history. It includes methods
to load, save, delete, and add, data on trails that the user has added, in a way that is aligned with 
the asynchronous examples given in class. It will be integrated into the Insights component and add trail component. 
**Point Value**: 5 
**Completed By**: Blake Thomas

## Feature: About Page 

An about page that provides information on the application and its core features. It will be integrated into 
the home page and bring the user into a separate page when clicked. It can include data on user amounts, 
location, and demographic. 
**Point Value**: 2 
**Completed By**: Blake Thomas

## Home Page
This is a page that contains all the buttons for our application. Includes CSS and connecting all components onto one page. the page will dynamically resize so that it can be used on multiple different device types, and look visually appealing for the user to easily access whatever they wish to access on the site.
**Point Value**: 4
**Completed By**: Will H and Will P 

## Home Icon Button
This feature allows users to navigate easily throughout the web app. For each component, there will be a home icon that the user can press to take them back to the main page.
**Point Value**: 2
**Completed By**: Will P

## Dark Mode
This feature is used as an additional option for the user to personalize their profile. They will be able to enable a "dark mode" toggle, where all colors will be inverted. Works on every page and every component in the sidebar, taking into account different styling types between the components so that there are no inconsistencies.
**Point Value**: 3
**Completed By**: Will P

## Google Maps Integration
This feature utilizes the Google Maps API to source and display hiking trails. Users can search or select a trail 
from a map interface to begin their journey. This integration provides a user-friendly way for hikers to discover and plan their routes, ensuring they have accurate and up-to-date trail information before setting out on their adventure.  In addition, the API also provides the closet shelters in case of any emergency (e.g landslide, flood, etc.). This will be done on the backend side. For now, it will be an option to "click to add your trail" with an image of Google Maps, as without the API, the trail cannot be looked up.
**Point Value**: 2
**Completed By**: Will P

## Add Emergency Contact: 
- The Add Emergency Contact feature provides users with the ability to store and manage emergency contact information within the application. When users need to input emergency contact details, they must provide three pieces of information: a first name, last name, and email address. The feature implements a form system that ensures data validity before storing the information in IndexedDB for persistent storage across browser sessions. To maintain data integrity  the system requires all form fields to be completed before submission is allowed. The email validation system uses regex pattern matching to verify that provided email addresses conforms to standard email formats, preventing invalid data from being stored. Once validated, the contact information is stored in IndexedDB, ensuring the data persists even after the browser is closed. In the case a user incorrectly inputs their data they will be alerted by an error message that says "Please fill in all fields." or "Please enter a valid email address", helping users correct input errors immediately, improving the overall user experience.. 
- When a user inputs their data it will be instantaneously added to the UI. 
**Point Value**: 3
**Completed By**: Ben Thomas

## Clear Emergency Contacts: 
- The Clear Emergency Contacts feature implements a data management system that enables users to remove all emergency contact records from both the user interface and persistent storage. This feature goes beyond simple UI deletion by also wiping the data from indexedDB. When the clear button is clicked the UI will instantaneously remove your emergency contacts.
**Point Value**: 3
**Completed By**: Ben Thomas

## Emergency Contacts UI:
- The Emergency Contacts UI feature implements a data visualization and management interface that demonstrates significant complexity through its real-time synchronization between the UI and IndexedDB persistent storage. 
- When the user accesses the application or refreshed, the system will immediately grab the data from IndexedDB and display it to the user. 
- When a new contact is added through the input form, the system not only persists this data to IndexedDB but also triggers an immediate UI update through the event system, ensuring the display reflects the current state without requiring a page refresh. All while managing different possible errors and protecting data integrity. 
- When users activate the clear functionality, the system coordinate numerous operations: initiating a database clear transaction, awaiting successful completion, and then instantly updating the UI to reflect the empty state. 
- By interacting with User Interface on a single render the user is capable of causing the system to apply 3 different calls on IndexedDB: .getall, .clear, .add
- Further, beyond the different functionalities the Emergency Contacts UI displays contact information in a clear, organized format while providing instantaneous visual updates whenever users add or remove contacts.
**Point Value**: 5
**Completed By**: Ben Thomas

## Add Start New Trail
The Add New Trails feature allows users to create and save detailed trail information for their backpacking adventures. This includes specifying the trail name, start and end locations, and uploading a relevant image for the trail. It also calculates the distance between locations (currently using a mocked value) and ensures all data is validated before being saved. This feature integrates seamlessly with the application's trail management system to store and display user-added trails.
**Point Value**: 3
**Completed By**: Nhan Daon

## Gear Recommendation
This feature uses a weather API based on location data to recommend a packing list of gear. For example, 
if the forecast predicts snow and cold weather, it provides the hiker with a cold weather packing list fit 
for those conditions. This helps ensure that hikers are properly equipped for the conditions they'll encounter, 
enhancing both comfort and safety.
**Point Value**: 3
**Completed By**: Dongpei Zhang

## Social Features 
Planned on making a page that allows users to add friends by their user id's and possibly even chat with them but was unable to make the 
indexedDB work and therefore we could not add features that rely on user ID. The storeFriend function is not working properly. it is being called but
it is not storing in indexedDB

**Point Value**: 3
**Completed By**: Will Hammond
