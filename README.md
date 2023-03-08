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




### <br>Time travel (Through commits)</br>

##### How we can move between the different commits that we have registered, suppose we have the following commits:

>   <br>f82f457 (HEAD -> master) more commands added</br>
>   <br>f52f3da new commands in fundamentals.md</br>
>   <br>e4ab8af my first commit</br>

#### We travel to the specific commit f52f3da
```
git reset --mixed f52f3da
```
#### We travel to the specific commit f52f3da and remove future changes
```
git reset --hard f52f3da
```
#### Show all changes even if we delete commits
```
git reflog
```
#### We travel to the specific commit f52f3da and we can restore the files
```
git reset --hard f52f3da
```
#### If we didn't commit but still want to revert the changes to a specific file we could use the following command:
```
git checkout -- fileName.withExtension
```
#### If we want to destroy all the changes without having made a commit we can use:
```
git reset --hard
```









