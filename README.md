

##Personal Website Lab

* First things first, click on the fork icon at the top of the page, then fork this lab by clicking the "Fork" button in the top right corner. 

* A copy of this lab now exists on your github account, but we need to clone the project to get it on your computer. 

* In the right navigation bar you should see something that says SSH clone URL and a link that starts with git@github... (if you don't see this you should click on the blue SSH link). You'll need that git@github link for the following command in your terminal:

`git clone git@github.com:<your username>/hs-git-website-lab.git`

* This will create a copy of the lab locally on your computer.

* Now that we have a local copy, we can cd into the project `cd hs-git-website-lab` and begin working on the lab!

* Let's make an `index.html` page for our site in this directory and open it up in Sublime Text.

* Now let's add some basic html. You can copy and paste this code into your index.html file:

```
<html>
  <head>
  <title> My Site </title>
  </head>
  <body>
    <h1> My Site </h1>
    <img src="http://i.telegraph.co.uk/multimedia/archive/01455/cat_1455103c.jpg"></img>
  </body>
</html>
```

* Let's see if git noticed that we added a file and made changes to it. Remember how to do that?

* We're finished with that part for now, so add and commit. Don't forget your commit message!

* Now let's push up our files to Github.com, so everyone can see what we've been working on, and if anything ever happens to our computers, our code is still accessible.

* First use `git remote -v` in the command line to make sure that the link to your github repo is set up properly. You should see `git@github.com:<your username>/hs-git-website-lab.git`.

* Do you see that? Great! Go ahead and push up to your fork.

* Now let's do some work on the header. We don't want to do work on the master branch though, right? Go ahead and create a new `header` branch and move to that branch.

* Before we get started working let's take a look at index.html in our browser. You can open it up in your browser by typing `open index.html` from the command line. 

* You should see 'My Site' for now, but let's make the site your own! Replace 'My Site' in the `<title>` and `<h1>`, tags with your name. 

* Refresh the page in your browser. Do you see your name?

* We eventually want to add a sub-header and a description, but we don't have enough time right now. We want to save our work though, so go ahead and add and commit these changes. 

* Now let's go back to master branch and open `index.html`. You'll notice your name no longer appears in the browser. Those changes only exist on the `header` branch. To see those changes on the master branch we need to merge the header branch into the master branch. Do that now.

Now if we reload index.html in the browser, you should see your name in the header.

Great job! 


### Wrapping up

Now that you completed the lab, make sure all your code is pushed up to your fork of the repository on Github. After that, we're going to create a pull request. A pull request is best practice for submitting contributions to an open source project. This is also how we'll be able to review your work and give you feedback on your code. 

* To create a pull request, go to your fork on the github website. 

* Click the green button in the top left corner. 

* On the next page, enter a comment for the pull request, like "completed lab" and click submit.

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/hs-git-website-lab' title='Personal Website Lab'>Personal Website Lab</a> on Learn.co and start learning to code for free.</p>
