# CS-360
Mobile Architect &amp; Programming
=======================================================================================================================================================================
Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?
The final project for this course that I chose was the first option available and that was to develop an inventory app that allowed for the management of an inventory. The items needed to be stored in a database, a database was needed for logging in and for adding new users, and the items being stored in the inventory database needed to be able to be added, removed, and the quantity altered. There also needed to be a settings screen that allowed for an sms message to be sent when an item ran out.
-
What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?
For logging into the app there needed to be an editable text box for the username and password, allow for the addition of new users to log into the system, and a warning to be displayed if the username and password were incorrect.
For using the app there needed to be the ability to handle an unknown amount of items, so I went with a recycler view that had a row for each item. The row allowed for the editing of the quantity of items, as well as the deletion of items. The main screen also needed to allow for the creation of a new item and the navigation to the settings screen.
For the settings screen there needed to be the ability to set up the sytem to send a text when an item ran out in the database of items. This I accomplished with a checkbox for sending sms messages and an editable textbox for entering a phone number.
-
How did you test to ensure your code was functional? Why is this process important and what did it reveal?
I ran through the functionality of the app personally to test the application, as well as purposly made errors and went through the various different steps a user could take (not just the steps I meant for users to take). This revealed that there was a bug in the code that if a user had allowed for sms messaging but hadnt entered a phone number, then the app would crash when an item reached 0 since it tried to get text from a null string. To fix this I added a second check before sending a message, that checked to make sure that the phone number was not null, and not emnpty.
-
Considering the full app design and development process, from initial planning to finalization, where did you have to innovate to overcome a challenge?
I had to innovate at the final stage of the development for me. I could not for the life of me get root preferences to work and I was unable to find assistance that showed how to communicate between root preferences and the main activity. To still accomplish my goal I switched and used a fragment as my settings screen and stored needed variables in the main activity and used interactions to communicate back and forth.
-
In what specific component from your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?
I am especially proud of the recyclerview that I set up. It is always kept updated with the database, allows for easy changing of the databasee, and can handle an infinite number of items since recyclerviews are scrollable. Each row is identical and the system is moduable and scaleable. By altering the row I could take the framework I set up and store any kind of list items that I might want with little change and lots of ease.
-
