# Barebones setup to get a working a minimal Node.js app working on Heroku

## Requirements

* Github
* Heroku Toolbelt
* Node.js


## Steps

1. Make sure you have a Github account setup as well as Heroku Toolbelt and Node installed.
2. Download the files at https://github.com/fulltilt/TestHeroku onto your filesystem.
3. Type ```npm install```
4. Go into the directory with the downloaded files and issue the following commands to initialize the Git repository:

 ```
 git init

 git add --all

 git commit -m 'Initial commit'
 ```

5. To connect the repository to Heroku type in the following commands:

 ```
 heroku create

 git push heroku master
 ```

If everything worked out, a bunch of Heroku logging messages should start printing out and near the end of it should be a cryptic url. Copy and paste that url into a browser and you should see the words "Hello World!"
6. You can make edits to the index.html file and to push your changes to Heroku:
 
 ``` 
 git add --all

 git commit -m '[some message describing your updates]'
 
 git push heroku master
 ```
 
 As is, you only have a single page to work with and if you want to add more pages to your app, you need to create routes which is beyond the scope of this tutorial.


## File info
* web.js: main file which you're app is run
* package.json: file listing dependencies of your app. What ```npm install``` looks at when install dependencies
* Procfile: command instructing Heroku to run. Similar to typing ```node web``` locally
* index.html: HTML for your app

NOTE: I typed this up in like 20 minutes and I could be off on a lot of things.