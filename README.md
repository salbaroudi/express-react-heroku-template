## Steps for launching a Heroku App:

000) Sign up for Heroku, setup 2FA, install on your desktop.

00) Run *heroku login* on command line, and connect. Login through your default browser, and then return to the commandline.

0) Make sure this project is uploaded to its own github repository before you start.

1) Now Adjustments to our App need to be done:

  a) Adjust the fetch() URL from *"localhost:3000"* to *`${document.location.origin}`*.

  b) Add an environment generated port number to index.js: with *const PORT = process.env.PORT || 3001;*

2) Once changes are complete, commit changes to github repository one more time.

3) Create a heroku remote repo with *heroku create*.

4) Run *git push heroku main* to run the application in the cloud.

5) run *heroku open* to see your new app in the browser.

## Editing Auto-Generated URL in Heroku:

1) The randomly generated application URL will not be desirable for your app. On the website, go into settings and customize
your url.

2) Git remote URL needs to be updated after this. Type: *git remote set-url <new heroku url>*

## Updating your app:

0) Login to heroku.

1) Run *git push heroku main*
