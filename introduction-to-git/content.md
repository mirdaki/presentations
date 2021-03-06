# Introduction to Git

### A better way to manage your code

<hr>

<small>By [Matthew Booe](http://www.matthewbooe.com)</small>



## Before we start

- Have Git installed
	- [git-scm.com/downloads](https://git-scm.com/downloads)
- Have a GitHub account
	- [github.com/](https://github.com/)


## About me

- Open Source Club founder
- GitHub Campus Expert
- Microsoft intern
- Star Wars lover

Note:
Establish credibility, but still appear human



## What's the problem?

<img class="r-stretch" src="https://cdn.images.dailystar.co.uk/dynamic/169/photos/707000/936x622/603707.jpg" alt="Man hanging from cliff">


## Sharing Code

- Email
- Flash drives
- Zip folders
- Cloud hosting

Note:
Poor alternatives


## Issues

- Track changes
- Backups
- Collaboration

Note:
- Track changes to "go back"
- Backups in case computer dies
- Collaboration to not get in the way and manage multitasking



## Introducing Git

<blockquote>
	"Git (/ɡɪt/) is a **version-control** system for tracking changes in computer files and coordinating work on those files among multiple people."
	<hr>
	<cite>Wikipedia</cite>
</blockquote>

Note:
Aww yes, of course! Insert laughter


## Version Control

- Track versions of code
- Resolve conflicts
- Provides workspace
- Backup server

Note:
Many version control systems like SVN and Mercurial


## Git

- Version control
- Open source
- Cross platform
- Distributed

Note:
- First created in 2005 by Linus Torvalds
- Distributed means that you don't need a server and can easily use multiple (or even just the same) computers


## Yeah, but what is it?

- Computer software
- Server software
- Collection of objects
	- In `.git` folder


## How to use Git?

- Need a Git _repository_
- Command Line
- GUI
	- GitHub Desktop, GitKracken, VSCode

Note:
Often call a repository a repo


## Hosting a repo

- Built in Git server
- GitHub
- BitBucket
- GitLab

Note:
Many others too


## What is GitHub?

- Hosted Git service
- Collaboration tools
- Online community
- **Not the same as Git**

Note:
- Lets other users discover and work on your project
- Great for open source projects
- Collaboration
	- Issues, Project Boards, Milestones, Pull Requests, Code Reviews, User Management, Organizations



## Git Workflow

<img class="r-stretch" src="https://www.novatec-gmbh.de/wp-content/uploads/2013/07/logo-git.png" alt="Git logo">


## Basic Steps

1. Change files
2. Let Git know
3. Package changes
4. Send to server


## Commit

- Collection of changes
- Message
- Metadata

Note:
The metadata contains things like author email, name, etc


## Branch

- History of commits
- A workspace
- Can diverge and _merge_ back

Note:
- Reminder, commit means changes, so it's a history of changes
- Commits point back at where they're from, like a linked-list
- Workspace as a way to focus on an issue or not mess with others
- Merge is a command you'll use


## More Branch

<img class="r-stretch" src="https://blog.seibert-media.net/wp-content/uploads/2015/07/Git-Branches-3.png" alt="Simple Git Branch">

Note:
Each points back to it's parent


## Even More Branch

<img class="r-stretch" src="https://blog.seibert-media.net/wp-content/uploads/2015/07/Git-Branches-1.png" alt="Regular Git Branch">

Note:
Multiple branches with their own histories


## Repository

- Collection of branches
- Store of objects
- Local or remote

Note:
Store of objects is just how Git tracks everything


## The "Buckets"

<img class="r-stretch" src="https://rachelcarmena.github.io/img/cards/posts/how-to-teach-Git/general-drawing.png" alt="Diagram showing the Working Directory, Staging Area, Local Repository, and Remote Repository of a Git setup">


## Downloading

<img class="r-stretch" src="https://raw.githubusercontent.com/rachelcarmena/how-to-teach/master/git/clone.png" alt="Diagram showing a git clone interact with the Working Directory, Local Repository, and Remote Repository of a Git setup">


## Workflow

<img class="r-stretch" src="https://raw.githubusercontent.com/rachelcarmena/how-to-teach/master/git/add-commit-push.png" alt="Diagram showing a git add, commit, and push interact with the Working Directory, Staging Area, Local Repository, and Remote Repository of a Git setup">


## Updating

<img class="r-stretch" src="https://raw.githubusercontent.com/rachelcarmena/how-to-teach/master/git/pull.png" alt="Diagram showing a git pull interact with the Working Directory, Local Repository, and Remote Repository of a Git setup">


## Checking

<img class="r-stretch" src="https://raw.githubusercontent.com/rachelcarmena/how-to-teach/master/git/states.png" alt="Diagram emphasizing the difference between the Working Directory, Staging Area, and Local Repository and the commands to diff them">



## Demo Time <!-- .element: style="color: #E74727;" -->

<!-- .slide: data-background-image="https://www.britspirit.co.uk/resources/walking-stick_defence_barton-wright_9.gif" data-background-size="70%" -->

<!-- The Gif is done kinda hack-y to make it big enough -->

Note:
- Btw, this is the "walking stick defense"
- Clone the repo
- Make a change
- Status
- Commit
- Push



## Configuring Git

It won't hurt a bit!

Note:
- I do want to apologize for that very intentional rhyme
- Also time to open up your terminal or Git bash


## Username

`git config --global user.name "<Name>"`

Note:
Do use your GitHub username


## Email

`git config --global user.email "<Email>"`
<br>
<br>
Check: [github.com/settings/emails](https://github.com/settings/emails)

Note:
The email will be public so I recommend going here and look under "Keep my email address private" for a fake one


## Editor

`git config --global core.editor "nano"`
<br>
<br>
**or**
<br>
<br>
`git config --global core.editor "notepad.exe"`

Note:
Nano is a CL text editor on Linux and MacOS and notepad.exe for Windows (other text editors should work too)



## Git Practice <!-- .element: style="color: #E74727;" -->

<!-- .slide: data-background-image="https://66.media.tumblr.com/3c451c21479835579118ff84a97c5976/tumblr_ouvxc3O5Gb1qbrivdo1_500.gif" data-background-size="80%" -->


## Fork a Repo

Forking copies the repo
<br>
<br>
Go here: [github.com/ufosc/practice-repo](https://github.com/ufosc/practice-repo)

Note:
- Forking is a GitHub feature, not native to Git
- This repo is provided by the Open Source Club for people to practice without worry


## Clone

Cloning downloads a copy
<br>
<br>
Run: `git clone <Git URL>`

Note:
- Do not download the zip, doesn't have the .git folder
- Download file to current shell location
- Git Bash on Windows sometimes has issues cloning. Closing and reopening fixes this


## Status

Check the repo's status
<br>
<br>
Run: `git status`

Note:
- Remember to change to the directory first
- This is a good command to run all the time


## Do Work

Add a file

Note:
Don't need to think to hard about it


## Add

Add the changes to Git's staging area
<br>
<br>
Run: `git add <filename>`

Note:
- Git will package all the things in staging
- Have to add files every time you want to record a change


## Commit

Commit to the changes
<br>
<br>
Run: `git commit`

Note:
- Please give a descriptive title
- Can add new lines to provide better description


## Pull

Pull down updates
<br>
<br>
Run: `git pull`

Note:
- This will let you know if anyone has updated it
- Keep in mind git status doesn't check the server, just what you know locally


## Push

Push your code up
<br>
<br>
Run: `git push`

Note:
- This will move your commit up to the server


## Success!

<img class="r-stretch" src="https://i.telegraph.co.uk/multimedia/archive/03596/Success_Kid_3596018k.jpg" alt="Succsess Kid">



## GitHub Practice <!-- .element: style="color: #E74727;" -->

<!-- .slide: data-background-image="https://media.giphy.com/media/a0QlNFxlTCba8/giphy.gif" data-background-size="90%" -->


## Edit Files

Single files can be edited and committed

Note:
Click the pencil icon


## Submit a Pull Request

Ask the original owner to pull in your changes

Note:
- Look at the branches to see what's happening
- This provides some access control
- Owners can choose to accept, ask for edits, or reject


## Issues

- Bug reports
- Feature requests
- Discussions

Note:
- This is a great way to list items that are TODO
- Assign people to them
- Add labels for easy organizing



## Other Things

<img class="r-stretch" src="https://openmatt.org/wp-content/uploads/2015/11/octocat_kenobi.jpg" alt="Obi-Wan Octocat">


## GitHub Info

- Tons of projects
- Not all necessarily open source
- Other tools
	- Projects, logs, milestones, wikis

Note:
- Check the license to see how you can use it


## Common Files

- README
	- Description of project
- LICENSE
	- Defines code usage
- CONTRIBUTING
	- Explains expectations for changes

Note:
- They are all capital to get your attention
- README also has info on running the project


## Git Flow

- "master"
	- Stable
- "dev"
	- Future stable
- feature-branch
	- Current work

Note:
- Use different branches to organize
- Multiple feature branches at the same time
- One issue per branch is a good rule


## Git Flow

<img class="r-stretch" src="https://blog.xebia.fr/wp-content/uploads/2018/03/Image.png" alt="Git Flow Example">


## Merge Conflict

Occurs when histories conflict

```JavaScript
<<<<<< HEAD
var left = true;
======
var right = true;
>>>>>> 6fc454c7bc33ca31d2e47d26762819e26a054534
```

Note:
- Star Wars analogy (we both saw original movie, but I saw prequels and you saw the rest of the originals)
- Just re-commit and megre



## Questions?



## Resources

- Free stuff: [education.github.com/pack](https://education.github.com/pack)
- Training lab: [try.github.io/](https://try.github.io/)
- Inner-workings of Git: [rachelcarmena.github.io/2018/12/12/how-to-teach-git.html](https://rachelcarmena.github.io/2018/12/12/how-to-teach-git.html)
- Presentation source code: [github.com/mirdaki/presentations](https://github.com/mirdaki/presentations)


## Thank you!

<img class="r-stretch" src="https://pbs.twimg.com/media/DfbsmMeU0AAIpmw.png" alt="Clippy and Mona">
