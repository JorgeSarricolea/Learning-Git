# What is GIT?

##### I like to say that it is like a super power of a developer or programmer. It is a **version control software**, its purpose is to keep track of changes in computer files (local level) and coordinate the work that several people do on shared files (You can also work alone, no problem). Now if you want to work remotely for that there is GitHub.

##### Click here to [Install Git](https://git-scm.com).

# What is GITHUB?

##### It is a collaborative development platform or as I like to say it; "The social network of a programmer" that is used to host projects (in the cloud) using the Git version control system. It also has a very useful tool that is GitHub Pages where we can publish our static projects (HTML, CSS and JS or other types of projects) for free.

### GIT Fundamentals and basic comands

#### Let's learn the first commands with GIT


#### To display the git version
```
git version
```

#### Register new user associated with GIT:
>   WARNING. Don't put the email of your Github account as a username, it could cause problems in the future.
```
git config --global user.name "my name"
```
#### It is recommended to use the mail associated with Github
```
git config --global user.email "myemail@example.com"
```
#### To get help 
```
git help
```
#### My first repository. Start a new repository and create the hidden .git folder
```
git init
```
#### See which files have not been registered
```
git status
```
#### Add all files to watch for changes
```
git add .
```
#### Create commit (current project snapshot)
```
git commit -m "my first commit"
```
#### Show the list of commits from newest to oldest
```
git log
```
##### In conclusion, we make changes to our files, the status command will verify which files have been modified. When we want to register those changes we will have to add them with add . so you are ready to make a commit. The commit makes the copy of that instant to be able to go back in time if necessary.










