# YOUR PROJECT TITLE
EJ MUSIC CONCERT
#### Video Demo:  <URL  HERE>https://youtu.be/gCTiM_jYGmE
#### Description:
TODO
**EJ MUSIC CONCERT** is where various ariste from Nigeria come to perform in the United Kingdom and people from all works of life get to attend this events which holds yearly. 

What a fanatic way of ending the year with people from some selected  countries getting a ticket to come watch, sing along and dance with the artiste. 
This year I selected countries who can apply on my hompage. The countries listed are United kingdom,USA,Canada, Nigeria and Spain. 

EJ MUSIC CONCERT  has a homepage which contains HOME, CONCERT, CATEOGORIES, REGISTER,LOGIN, LOGOUT pages.
###### 
People  attending  EJ MUSIC CONCERT will use the homepage to register there details and we have some selected countries on my homepage.  

1.What each person need to REGISTER is:
   + Entering their username
   - Email Address
   * Enter their unique password
   - Retype their password
when a person REGISTER their details, they are automatically referred to a LOGIN page were they type their username & password

2.The CONCERT page shows the following information:
   + Name of Artiste
   - Month and Date of Performance
   * The Atriste Imaage
   - What songs each artiste would perform


3.The CATEGORIES have a drop down button that have

   * Regular
   * VIP
   * Ticket

   Under Regular 
   - Each person inputs their name and have select their country
   - Click the submit button
   - Click the home button to return to hompage

   Under Vip 
   - Each person inputs their name and have select their country
   - Click the submit button
   - Click the home button to return to hompage

  The Ticket option shows were people who choose the cateory they would prefer see their names. 
  People select their name, country and click on the submit button.The ticket is ready but people  getting the ticket,are excepted to click on home to take them back to the hompage.
  Also all names and countries are saved in a cache  

**Running**  
 Under my local Vscode i am running  WSL-UBUNTU.I used $ python3 app.py to run my program and I used Url to link my page to the browser.

**Understanding**
under the music folder we have  __pycache__, static and  templates subfolder

My homepage was built using HTML, CSS,Javascript also having __init__.py which contains the database using db =SQLalchemy()

auth.py

- Shows that all users details are authenticated using  POST when they login. And notice how it uses check_password_hash to compare hashes of users’ passwords. Also notice how login “remembers” that a user is logged in .That way, any of this file’s routes can check which user, if any, is logged in. Finally, notice how once the user has successfully logged in, login will redirect to #, taking the user to their home page. Meanwhile, notice how logout simply clears session, effectively logging a user out.
Notice too how most routes support GET and POST. 

models.py
- This section contains the database used to develop the project. it contains class Register, class Tickets,class Regular, class Vip,
class Concerts database

views.py
- Views all pages on EJ MUSIC CONCERT and has a return_template

Static/
- Glance too at static, inside of which is styles.css.That’s where some initial CSS lives.

Templates/
Now look in templates/. In login.html is, essentially, just an HTML form, stylized with Bootstrap. In apology.html, meanwhile, is a template for an apology.

In the concerts.html it has the link ref , style under it has script,body and a table.

The index.html is the hompage that has other pages embedded. It’s a bit bigger than usual, but that’s mostly because it comes with a fancy, mobile-friendly “navbar” (navigation bar), also based on Bootstrap.

Specification

Register
- Complete the implementation of register in such a way that it allows a user to register for an account via a form.

- Require that a user input a username, implemented as a text field whose name is username. Render an apology if the user’s input is blank or the username already exists.

- Require that a user input a password, implemented as a text field whose name is password, and then that same password again, implemented as a  text field whose name is confirmation. Render an apology if either input is blank or the passwords do not match.

- Submit the user’s input via POST to /register.

- INSERT the new user into users, storing a hash of the user’s password, not the password itself. Hash the user’s password with generate_password_hash Odds are you’ll want to create a new template (e.g., register.html) that’s quite similar to login.html.

- Once you’ve implemented register correctly, you should be able to register for an account and log in (since login and logout already work)!

Concerts
- Displays the artiste image, date, month, songs and tickets.

Regular
- Complete the implementation of Regular in such a way that it enables a person enter their details.Submit the user’s input via POST to /buy.
   Upon completion, redirect the user to the home page.


Index
- Complete the implementation of index in such a way that it displays an HTML table summarizing, for the user currently logged in, it displays all other pages such as Concerts, Categories,Register,Login and Logout.

Vip
- Complete the implementation of sell in such that people can input their name and country.
  Upon completion, redirect the user to the home page.

Tickets
- Complete the implementation of Tickets in such a way that it displays an HTML table summarizing all of a user’s details , listing their name and country.


