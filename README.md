---
  tags: git, kids 
  languages: git
  level: 1
  type: lab
---

## Using Git with Github

The goal of this lab is to get you comfortable using git and github.

* First things first, we need to create a directory for our project and `cd` into it:

`mkdir my_website`
`cd my_website`

* Now that we're in the project, we need to initialize a new git repository. Remember how to do that?

* Don't forget to also create a `README.md` file. Why is a README important?

`touch README.md`
`subl README.md` 

* Add some descriptive language to your README. Maybe something like this: "This is my personal website with a cat photo."

* Now let's see if git noticed that we made changes to our `README.md`. Remember how to do that? 

* Now that we've finished editing our README, let's stage and commit. Don't forget your commit message!

* Now let's push up our files to Github.com, so everyone can see what we've been working on, and if anything ever happens to our computers, our code is still accessible. 

* You should already have a remote set up, but let's check by using `git remote -v`. Do you see your fork? Go ahead and push up to your fork. 

* Now let's make the `index.html` page of our site.

`touch index.html`
`subl index.html`

* Now that let's add some basic html. You can copy and paste this code

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

* Then go ahead and add, commit and push.

* Let's do some work on the header, but we never want to do work on the master branch, right? Go ahead and create a new header branch and move to that branch.

* Before we get started working let's take a look at index.html in our browser. You can open it up by typing `open index.html` from the command line. 

* You should see 'My Site', but let's make the site your own! Replace that text in the `<title>` and `<h1>`, tags with your name. We should probably add a sub-header and a description, but we don't have enough time right now. We do want to save our work though, so go ahead and add and commit these changes. 

* We also want to push these changes to github but there is not a remote version of the branch on github. To push up our code we need to use this command:

`git push origin header`

The header branch didn't previously exist on github; so that last command explicitly tells git to push to the remote location (origin) our new branch (header). 

* Let's go back to master branch now and open `index.html`. You'll notice your name no longer appears in the browser. Those changes only exist on my `header` branch.

* We're done making changes for now though so go ahead and merge the header branch into the master branch.

Now if we reload index.html in the browser, you should see your name in the header.

Great job! 


### Wrapping up

Now that you completed the lab, make sure all your code is pushed up to your version of the repository on github. After that, we're going to create a pull request. A pull request is the best practice for submitting contribution of work to an open source project. This is also how we'll be able to review your work and give you feedback on your code. 

* To create a pull request, go to your version of the repository on your github account. 

* Click the green button in the top left corner. 

* On the next page, enter a comment for the pull request, like "completed lab" and click submit.
