# myFirstRepo

Let's fork this repo and create your own branch!

We'll go by it step by step...


### Step 1
Click the "Fork" button on the repo's main page, and follow the prompts to fork the repo into your own account. In this context, "forking" effectively means copying an existing GitHub repository as your own to work on via your own account. Changes to a forked repo will not change the original.

### Step 2
Click the "Code" button in your own repo, and you'll see a drop down menu with the option to clone via HTTPS, SSH or GitHub CLI. We're going to clone via HTTPS, so all you need to do is copy the address provided above the text "Clone using the web URL."

### Step 3
Go to your terminal, and navigate to a folder you want to clone the repository into.

### Step 4
Let's first initialize the folder as a git project by typing:
  ```
  git init
```
If successful, you should see the message:
> Initialized empty Git repository in ```(whatever directory you set)```

### Step 5
Now we want to attach your current folder to your new repo. Remember the address you copied in step 2? Now we're going to use it here! We're going to use the ```remote``` command in git, which will establish where our repository code originates from! You'll want to enter the following, replacing ```PATH``` with whatever address you copied in step 2:
```
git remote add origin PATH
```
If it worked, you _won't_ receive a confirmation message.

### Step 6
If you haven't set a global user config for your Github account, you can set up a local credential in your terminal now. **SKIP THIS STEP IF YOU'VE ALREADY SET GLOBAL CREDENTIALS**
In your terminal, set your user configuration using the following, replacing USERNAME and EMAIL with your actual GitHub username and email address:
```
git config --local user.name USERNAME
git config --local user.email EMAIL
```
This will connect your account specifically with the folder we've initialized. This is only necessary if you're juggling multiple GitHub accounts and don't want your other accounts to intefere. Otherwise, using your global config is fine!

### Step 7
Now for the first step: Pulling data from the repo! Git works through the concept of pushing and pulling. **Pushing** data means uploading changes you've made on your local machine to the remote repository on GitHub. **Pulling** data means _downloading_ the current state of the remote repository to your local machine. Since our working folder is currently empty, we'll need to use the ```pull``` command. And when we're making our first pull, we need to specify that we're pulling from the MAIN branch of the ORIGIN (root). The command we'll use therefore is:
```
git pull origin main
```
If successful, you'll have downloaded the contents of your repo and be ready to work!

### Step 8
Not really a step, but to confirm your local folder matches the repo, try the following:
```
git status
```
You should see something along the following:
```
On branch main
nothing to commit, working tree clean
```
This means our copy is complete, and our local folder matches the remote repo exactly!

### Step 9
You did it! On your repo's main page on GitHub, click the Code button again, and copy the HTTPS address of your own forked repo (not the original). Submit it on Blackboard, and enjoy the rest of your week! 🎉