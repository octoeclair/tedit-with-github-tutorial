#Collaborating with Github and Tedit - A Simple Tutorial
#####**Tutorial in progress**
###How to Clone a Repository
1. Download Tedit at https://chrome.google.com/webstore/detail/tedit-development-environ/ooekdijbnbbjdfjocaiflnjgoohnblgf?hl=en-US
2. Right click on Tedit and select the option that says "Clone Github Repo".
![Clone Github Repository](https://raw.githubusercontent.com/octoeclair/tedit-with-github-tutorial/master/imgs/tedit-tut-clone-git.png)
3. You should get a prompt box looking like this:
![Empty Fields](https://raw.githubusercontent.com/octoeclair/tedit-with-github-tutorial/master/imgs/tedit-tut-1-empty-fields.png)
4. The following steps assume you have already created a repository on Github. If you haven't, click [here](https://help.github.com/articles/create-a-repo/) before continuing.
5. Fill out the fields
  1. Fill out the "user/name" box with your username followed by a slash and then the project name. If I wanted to clone my domcg repository, the box would be filled out with "octoeclair/domcg".
  2. Ignore the "ref/heads/master" field.
  3. You can optionally fill in the "localname" field with the name you want the repository to be called on your computer. If you leave this blank, it will be the actual name (the name on Github). I want domcg to be called "dominion" so I'll write that.
  4. Leave the encryption passphrase blank.
  5. This is the tricky field! If you have a Github Auth Token, copy it and paste it here. You likely don't, so create one [here](https://github.com/settings/tokens/new). After you enter your password, select these checkboxes ![Checkboxes](https://raw.githubusercontent.com/octoeclair/tedit-with-github-tutorial/master/imgs/tedit-tut-genauthtoken-scopes.png). Click "Generate token" and copy the token they give you. **Do not copy any white space** *and do not lose the token.* the token will not work with leading or trailing spaces, and Github will not let you see the token again after you leave the page.
  6. Paste the token into the "Enter github auth token" field.
6. The box should look similar to this (I didn't show my auth token for security reasons). ![Final](https://raw.githubusercontent.com/octoeclair/tedit-with-github-tutorial/master/imgs/tedit-tut-filled-fields.png)
Of course, the exact values of the fields will be different for you as you use Github for different things, but you get the idea. If the box looks something like the example above, click "OK".
7. Congratulations, you have successfully cloned your first github repository!

###Pulling, Committing, and Pushing
In a nutshell, if you and your friend are working on one project, there are essentially three different git repos being used.
One is the repo in your Tedit Developer Environment, the other is the repo in your friend's computer, and the final one is on Github. Luckily, all your repos are connected by a *remote*, so you can collaborate. Every time you make edits, you should follow this process.

1. *Pull* in the newest version of the project by right-clicking on the repo folder and selecting "Sync with Remote". This is important, because the version of the repo you might be working on might be outdated. That is, your friend might have made some changes since the last time you worked on the repo. *Your repo doesn't update automatically, you have to explicity pull changes (update it) yourself!*
  1. If the editor says something like "No changes to sync." you are good to go! It means you are up to date and have no changes to pull.
  2. If the editor opens a prompt box like this, ![Pull Changes?](https://raw.githubusercontent.com/octoeclair/tedit-with-github-tutorial/master/imgs/tedit-tut-im-behind.png) simply click "Yes" and Tedit will update your repo.
2. Edit. Create files, edit files, delete files, do whatever you want. When you feel like you are at a good stopping point, move on to the next step.
3. *Commit* your changes. Changes are grouped into *commits*. Instead of updating the main repo on Github everytime you change a single character, you organize related changes into *commits*, and push commits instead. This everything a lot more organized. ![Why Git Uses Commits Meme](https://raw.githubusercontent.com/octoeclair/tedit-with-github-tutorial/master/imgs/Why%20Git%20Uses%20Commits.jpg)
  To commit your changes, right click the repo and select "Commit Changes". ![Select Commit](https://raw.githubusercontent.com/octoeclair/tedit-with-github-tutorial/master/imgs/tedit-tut-6-commit.png) You should get a prompt like  this. ![Commit Form](https://raw.githubusercontent.com/octoeclair/tedit-with-github-tutorial/master/imgs/tedit-tut-commit-empty-fields.png)
  1. Write a short summary of what you changed in the "Details about commit." field. Like I previously mentioned, related edits should be grouped together in the same commits. If you followed my advice, your changes should be related and it should therefore be easy to summarize the commit. Good commit descriptions are short and descripted. For example, if you created a file called `index.html`, your description could simply be "Created index.html."
  2. Write your full name in the "Full Name" field.
  3. Write your email in the "email@provider.com" field.
  4. The box should look something like this (the exact field values will vary for each person, obviously) ![Filled Commit Form](https://raw.githubusercontent.com/octoeclair/tedit-with-github-tutorial/master/imgs/tedit-tut-committing.png)
  5. Click the "OK" button.
4. *Push* your changes. Right click your repo folder and click "Sync with Remote". ![Pushing](https://raw.githubusercontent.com/octoeclair/tedit-with-github-tutorial/master/imgs/tedit-tut-sync-remote.png) A prompt will be opened asking you to confirm the push. ![Confirm Push](https://raw.githubusercontent.com/octoeclair/tedit-with-github-tutorial/master/imgs/tedit-tut-push.png) Click "Yes".
5. Congratulations, you've just completed your first *pull, commit (sometimes multiple times), push* cycle!
