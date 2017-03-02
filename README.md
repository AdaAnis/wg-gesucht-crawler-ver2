# WG-Gesucht-Crawler
Crawls the WG-Gesucht site for new apartment listings and send a message to the poster,
based off your saved filters and saved text.

Uses Tkinter for the GUI and ~~MechanicalSoup~~ Selenium to crawl the site.

**Update**  
WG-Gesucht changed their login, making it not possbile to use MechanicanlSoup anymore,
so it now needs to use Selenium.

You can download the PhantomJS binary for you OS can be downloaded [here](http://phantomjs.org/download.html)

It then needs to be placed in the working directory in a folder named '.phantomjs' so the folder tree looks like:(should be already there)

Working Dir  
├── main.py  
├── .phantomjs  
│                     └── bin  
│                                          └── phantomjs (binary)  
└── wg_gesucht.py


## Use
Install the Python packages in the 'requirements.txt' and run then 'main.py'

Enter your email address and password that you use for wg-gesucht.de (will be saved
locally so you don't have to type it every time you run it)
Make sure you have 1 or more filters created and that you have saved a template text
on your wg-gesucht account.

Then just leave it running in the background, it will check for new apartment listings
every 5 minutes, and message any new ones that appear.

It will also create a folder with the apartment ads that you can view offline, in case
the poster removes their ad before you get a chance to look at it, which can happen
if the poster receives a lot a messages in a short amount of time.

P.S: This bases on the work of https://github.com/grantwilliams/wg-gesucht-crawler. Found some Issues, and I am still trying to troubleshoot them :)
