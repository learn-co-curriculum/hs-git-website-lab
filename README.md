---
  tags: git, kids 
  languages: git
  level: 1
  type: lab
---

The goal of this lab is to get you comfortable using git and github.

### So let's actually start a project.

First things first, we need to create a directory for our project and `cd` into it:

`mkdir my_website`
`cd my_website`

Now that we're in the project, we need to initialize a new git repository. Remember how to do that?

Don't forget to also create a `README.md` file. Why is a README important?

`touch README.md`
`subl README.md` 

Add some descriptive language to your README. Maybe something like this: "This is my personal website with a cat photo."

Now let's see if git noticed that we made changes to our `README.md`. Remember how to do that? 

Now that we've finished editing our README, let's stage and commit. Don't forget your commit message!

Now that git knows about our files, we're going to want to put it up on Github.com, so everyone can see what we've been working on, and if anything ever happens to our computers, our code is still accessible. You should already have a remote set up, but let's check by using `git remote -v`. Do you see your fork? Go ahead and push up to your fork. 

Now let's make the `index.html` page of our site.

`touch index.html`
`subl index.html`

Now that let's add some basic html. You can copy and paste from the code_for_homepage.html file in this directory. Then go ahead and 

`git add <file-name>`
`git commit -m "created index.html"`
`git push`

So far, we've been working on what's master branch. Master should always be the stable working version of your code. You never want to break master. Let's just confirm we're on master. Remember how to do that?

Now let's create our new feature branch. Let's call this branch "header", because we'll be working on a header feature for the site. Now if we check the branch, it should tell us we're on the header branch.

Let's take a look at index.html in our browser, by typing `open index.html` from the command line. You should see 'My Site', but let's make the site your own! Replace that text in the title and header, `<h1>`, tags with your name. We should probably add a sub-header and a description, but we don't have enough time right now. We want to save our work though, so go ahead and add, commit, and push these changes to a remote version of my branch.

`git add <file-name>`
`git commit -m "started working on header"`
`git push origin header`

The header branch didn't previously exist on github; so that last command explicitly tells git to push to the remote location (origin) our new branch (header). 

So let's go back to master `git checkout master` and open `index.html`. You'll notice your name no longer appears in the browser. Those changes only exist on my `header` branch.

Let's hold off on making any more changes to the header for the time being. We'll consider that feature complete. Go ahead and merge this branch into master.

Now if we reload index.html in the browser, you should see your name in the header.

Great job! Now that all of our changes are merged into our master branch, go ahead and push up your changes to github then open a pull request. A pull request is the best practice for submitting contribution of work to an open source project. To create a pull request, go to your version of the repository on your github account. We'll click the green button in the top left corner. On the next page, we'll want to enter a comment for the pull request, "completed lab" and click submit. This is how I'll be able to review your work and give you feedback on your code. 
