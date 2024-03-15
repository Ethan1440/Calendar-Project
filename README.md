# Calendar-Project
Simple calendar project developed for Solved. The calendar is only compatible with desktop screen sizes.

Notes:
-The script had to be cut from the html file as google and Windows Defender were flaging it with a false positive for viruses.
-Data is only saved in the instance the calendar has been loaded in. All tasks will be deleted each time the page is refreshed.
-I have mainly tested on google, but it also seems to work fine on Microsoft edge and Firefox. I would still recommend using google though.

##Running Calendar HTML
1. Unzip project files to your local drive and ensure the calendar.html file and all style sheets (.css) are in the same directory (folder)
2. Open the calendar_script.txt file and copy all of the text in that file to clip board (CTRL + A, then CTRL + C)
3. Open the calendar.html file with any text editor or code editor and paste (CTRL + V) the text between the script tags.     <script> PASTE HERE </script>
4. Save the calendar.html file
4. You should be able to open the calendar.html file in Google Chrome and it will launch in the browser. (double click file, or right click and open with google)
5. Alternate option for opening: If you want to see the calendar in live form you can also open it with Visual Studio Code, and use the Live Server extension to open the calendar.html file.

##Using the Calendar
* The arrows on either side of the month and year in the header will move forward or backwards a month
* the add assignment button will open a modal where you can fill out a task's details and add it to the calendar
* When more than 3 tasks are added to a single day, three dots will be placed on that day in the month-view to indicate the day contains more tasks
* each day in the month view can be double-clicked to open that day's day-view. Here each task for that day will be displayed
* In day-view, the x in the upper right corner of the task will remove the task from the calendar
* Error Checking
  * add assignment does not allow invalid dates due to the input method
  * The name and description are characters limited to 30 and 60 characters respectively
  * Tasks with the same name are not allowed on the same date

##Features
* Month-view can switch between months of the year
* Add and remove assignments from the calendar
* month-view indicates if the date contains more tasks than visible, also prevents tasks from being appended to the same day and running off the screen
* compatible across common desktop viewports
* January and December month grid generation edge cases addressed
* Today's date day is highlighted
* All Task data is required and validated
   * duplicate tasks are validated in the code
   * date is validated by the interface, does not allow invalid date to be entered
   * cannot add assignment if it does not have all fields filled out
