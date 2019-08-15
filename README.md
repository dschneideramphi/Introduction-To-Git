# Introduction-To-Git
Welcome! We will use this assignment to learn some new commands in a program called *Git*

## Step 0 - Getting Setup

We only need to do this step once for any project we ever do. We're setting up our author information as we make changes using git. To do this, run the following commands:

`git config --global user.name "[your-name]"`
`git config --global user.email "[your-email]"`

## Step 1 - Cloning

In your Cloud9 terminal, we will **clone** this Git Repository. You can do that by typing:

`git clone https://github.com/dschneideramphi/Introduction-To-Git`

Once you've done this, a new folder will appear in your Cloud9 environment called Introduction-To-Git. We'll need to use the `cd` command to do that:

`cd Introduction-To-Git`

**What's Happening:** Github is a website that coders use to store code so it can be easily shared and downloaded, and *Git* is a program & set of commands that lets coders manage their code. It helps them keep track of changes; it helps them keep track of which version they're on; it helps them collaborate together - it's super helpful. We've just used Git to download some code files called a **repository**. We're about to go through some steps where we can update and make changes to this set of code so everyone can see it.

## Step 2 - Contributing

You will make an Introduction File that we will add to this **repository**. Start by creating a new file using the `touch` command in the console. The file should be *[your_name].txt*

`touch [your_name].txt`

The file should appear in the Cloud9 file system. Double-click the file to open it.

Add the following 3 things to this file:

1) Your Name
2) Your Favorite Safari Animal
3) If you could have *any* superhero power, what would it be and why?

**Remember to Save Your File!**

## Step 3 - Comitting

Now that you've made a change to this *repository*, we'll need to let Git know about it. This process has 2 steps:
1) We need to **add** this new file to our Git repository. We can do this with the following git command:

`git add [your-name].txt`

2) We need to **committ** our changes, which saves them to the Git timeline. We can do this with the following git command:

`git commit -m "Added my file"`

**What's Happening:** Git keeps track of changes that have been made to code so you can see who has been updating the code, what's been changed, and how often changes have been occuring. These extra git commands are like adding an entry to a log-file of all the updates. Specifically:
- `git add` tells Git that you've been updating a file but aren't ready to totally commit it yet
- `git commit` tells Git that you're ready to create a 'snapshot' of all the files that have been added using `git add`

For now, all these updates are only happening *on your local computer* - in the next step, we'll merge them all back together on GitHub!

## Step 4 - Pushing

Now that we've made our local changes, it's time to push them back to our Git repository. We can do that with the following command:

`git push origin master`

**What's Happening:**
- `git`: tells the terminal to access the Git program of commands
- `push`: tells Git we're about to send changes out to Github
- `origin`: tells Git which **repository** to add our changes to. In this case, it's the same as where we downloaded it from
- `master`: tells Git to update the 'master' set of code. In larger projects, there are usually several **branches** of code that people are working on (like an *alpha* branch or a *test* branch). For most of our projects, we'll just have one set of code - the Master branch

## Step 5 - Pull

Finally, afyer everyone has pushed their code, let's look at the results by running this command:

`git pull origin master`

Watch what happens next...
