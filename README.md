# Job-Application-Autofill-Automation
Autofills and Automates filling out Job Apllications using Xpaths and python.

## Description

I was looking for a python program that would allow me easy quick change from career site to career site for automation. There wasnt
one that did what I exactly wanted. This program Opens a new browser window but will keep it open and only work inside that particular session
you can navigate around yourself and selenium and the chrome driver will stay connected to that session that opened instead of opening a new one.
This allows you to navigate a Career website live to different job applications and (run the last cell - input cell) and watch it fill out the app.
The only thing you really need to do is go through and grab the xpaths of all the cells on the path and change the keys depending on what the cell is
drop down or key input.

## Dependencies

###### ChromeDriver

https://chromedriver.chromium.org/downloads
Check your version of Chrome and make sure you grab the proper ChromeDriver per the version.

###### Selenium

pip install selenium

## Steps

1. Run the first cell. This will open your initial instance of chrome with one tab. This is the session we're going to work from
2. Next Run the second cell which should have the URL of an application on the job website your trying to automate. You should be able to watch the new URL load in the same session you initially opened. This is the magic of the second cell. From here if you need to log in to get to the applications you can otherwise continue. Everything you do in this window will be saved. This is our open and working connected session.
3. From here inside that session Inspect and copy the Xpaths of the inputs of each of the boxes for the Job Application. Most questions are the same per application so hopefully all you need to do is to paste the xpaths in the appropriate places such as name, email, phone number, website etc. Most application career websites are tricky but some have hidden elements that need to be clicked to reveal for you to get the xpath, some have elements on top of elements, and you'll need to figure out how to access the proper xpath for them.
4. Once you do one application you should be good to go, now click to the next application and only run the last cell where you changed the xpaths and it should autofill live while you watch. Continue to do this until all your applications are filled out. I usually only employ this if there are tedious sections as well as more then 5 applications I wish to fill.
