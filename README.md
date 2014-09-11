---
  tags: git, kids 
  languages: git
  level: 1
  type: lab
---

## Using Git with Github

The goal of this lab is to get you comfortable using git and github.

* First things first, fork this lab by clicking the `Fork` button in the top right corner. When you do that, notice the location of the new forked repository is <your github username>/hs-git-website-lab. A copy of this lab now exists on your github account.  

* Now we have to clone the project to get it on your computer. You should see something that says SSH clone URL and a linkt that starts with git@github... (if you don't see this you should click on the blue SSH link). You'll need that link for the following command in your terminal:

`git clone git@github.com:<your username>/hs-git-website-lab.git`

* This will create a copy of the lab locally on your computer.

* Now that we have it up locally, we can cd into the project `cd hs-git-website-lab` and begin working on the lab!

* First let's make a `index.html` page for our site.

`touch index.html`
`subl index.html`

* Add this file to make sure git is tracking your changes. Remember how to do that?

* Now add some basic html. You can copy and paste this code

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

* Now let's see if git noticed that we made changes to our index.html. Remember how to do that?

* We're finished with that part for now, so stage and commit. Don't forget your commit message!

* Now let's push up our files to Github.com, so everyone can see what we've been working on, and if anything ever happens to our computers, our code is still accessible.

* First use `git remote -v` in the command line to make sure that the link to your github repo is set up properly. You should see `git@github.com:<your username>/hs-git-website-lab.git`.

* Do you see that? Great! Go ahead and push up to your fork.

* Now let's do some work on the header. We never want to do work on the master branch though, right? Go ahead and create a new `header` branch and move to that branch.

* Before we get started working let's take a look at index.html in our browser. You can open it up by typing `open index.html` from the command line. 

* You should see 'My Site' for now, but let's make the site your own! Replace that text in the `<title>` and `<h1>`, tags with your name. 

* We eventually want to add a sub-header and a description, but we don't have enough time right now. We do want to save our work though, so go ahead and add and commit these changes. 

* Now let's go back to master branch and open `index.html`. You'll notice your name no longer appears in the browser. Those changes only exist on the `header` branch. To see those changes on the master branch we need to merge the header branch into the master branch. Do that now.

Now if we reload index.html in the browser, you should see your name in the header.

Great job! 


### Wrapping up

Now that you completed the lab, make sure all your code is pushed up to your fork of the repository on github. After that, we're going to create a pull request. A pull request is best practice for submitting contributions to an open source project. This is also how we'll be able to review your work and give you feedback on your code. 

* To create a pull request, go to your fork on the github website. 

* Click the green button in the top left corner. 

* On the next page, enter a comment for the pull request, like "completed lab" and click submit.
