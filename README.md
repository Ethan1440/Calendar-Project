# Calendar-Project
Simple calendar project developed for Solved. The calendar is only compatible with desktop screen sizes.

Notes:
Data is only saved in the instance the calendar has been loaded in. All tasks will be deleted each time the page is refreshed.
The script has to be included in the HTML document as you cannot link script files externally from a local storage system to the browser due to internet security.

##Opening Calendar HTML
1. Ensure the HTML file and all style sheets (.css) are in the same directory
2. You should be able to open the calendar.html file in Google Chrome and it will launch in the browser.
3. Alternate option: If you want to see the calendar in live form you can also open it with Visual Studio code, and use the Live Server extension to open the calendar.html file.

##Using the Calendar
* The arrows on either side of the month and year in the header will move forward or backwards a month
* the add assignment button will open a modal where you can fill out a task's details and add it to the calendar
* When more than 3 tasks are added to a single day, three dots will be placed on that day in the month-view to indicate the day contains more tasks
* each day in the month view can be double-clicked to open that day's day-view. Here each task for that day will be displayed
* In day-view, the x in the upper right corner of the task will remove the task from the calendar
* Error Checking
  * add assignment does not allow invalid dates due to the input method
  * The name and description are characters limited to 50 and 100 characters each
  * Tasks with the same name are not allowed on the same date

##Features
* Month-view can switch between months of the year
* Add and remove assignments from the calendar
* month-view indicates if the date contains more tasks than visible, also prevents tasks from being appended to the same day and running off the screen
* compatible across common desktop viewports
* January and December month grid generation edge cases addressed
