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

### How I can name my commits?
##### The Conventional Commits specification is a lightweight convention on top of commit messages. It provides an easy set of rules for creating an explicit commit history; which makes it easier to write automated tools on top of. This convention dovetails with SemVer, by describing the features, fixes, and breaking changes made in commit messages.

#### The commit contains the following structural elements, to communicate intent to the consumers of your library:

- [b]fix:[/b] a commit of the type fix patches a bug in your codebase (this correlates with PATCH in Semantic Versioning).

- feat: a commit of the type feat introduces a new feature to the codebase (this correlates with MINOR in Semantic Versioning).

- BREAKING CHANGE: a commit that has a footer BREAKING CHANGE:, or appends a ! after the type/scope, introduces a breaking API change (correlating with MAJOR in Semantic Versioning). A BREAKING CHANGE can be part of commits of any type.

- types other than fix: and feat: are allowed, for example @commitlint/config-conventional (based on the Angular convention) recommends build:, chore:, ci:, docs:, style:, refactor:, perf:, test:, and others.

- footers other than BREAKING CHANGE: <description> may be provided and follow a convention similar to git trailer format.

Additional types are not mandated by the Conventional Commits specification, and have no implicit effect in Semantic Versioning (unless they include a BREAKING CHANGE). A scope may be provided to a commit’s type, to provide additional contextual information and is contained within parenthesis, e.g., feat(parser): add ability to parse arrays.

### Did you create a new repository in GitHub and you want to connect it with your local folder?

#### Remember, fisrt command!
```
git init
```
#### After doing the "First commit" you will write the next 3 commands:
```
git branch -M main
git remote add origin https://github.com/Your-User-Name/Name-Of-Your-Repository.git
git push -u origin main
```
##### And that's it, you push your local repository to GitHub!

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


### <br>Modify files</br>

##### We may want to rename a file, it is recommended to do it directly on the command line to register the changes with git.

#### Change file name. 
```
git mv originalName.vue newName.vue
```

#### Delete files
```
git rm fileName.vue
```
#### Ignoring Files

##### In order not to track folders or files, we must create the following file: .gitignore. Your example structure would be like this:
```
file.js // Ignore the file in question
*.js // Ignore all files with .js extension
node_modules/ //Ignore the whole folder
```


### <br>Branch</br>

##### So far we have only worked on the "master" branch but we may need to create different branches for git traces.

#### Create a new branch
```
git branch branchName
```
#### It shows us in which branch we are
```
git branch
```
#### We move to the new branch
```
git checkout branchName
```
#### We can merge the master branch with the new one. We move to the new branch
```
git merge branchName
```
#### Delete a branch
```
git branch -d branchName
```


### <br>Tags</br>

##### With the tags we can make versions of our project.

#### Create a tag
```
git tag alphaVersion -m "alpha version"
```

#### List tags
```
git tag
```

#### Delete tags
```
git tag -d tagsName
```

#### Make a version on a previous commit ex: f52f3da
```
git tag -a tagName f52f3da -m "version alpha"
```

#### Show tag information
```
git show tagName
```













