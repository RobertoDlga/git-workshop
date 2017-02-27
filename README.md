# Git Workshop: The Basics

With the following steps you will learn what `git status`, `git add` and `git commit ` do and what `tracking`, `untracked` and `staging` means.

Open your terminal and your favorite editor and follow this steps:

### Set up your project with git

1. Create a folder for your project. `mkdir git-workshop && cd git-workshop`
2. Run `git init`.
  * This command will initialize your folder as a git repository.
  * You can see a hidden `.git` folder. Here is where git does it's magic.

Done! Now your project is ready to use git.

### The basic workflow

Now we will do the basic workflow of adding and commiting a new file to track a change over time. This is the very first step to start using git.

3. Run `git status`.
  * This command shows you the `status` of your project. Meaning that it will show you what files have changed and what is ready to be commited.
4. Create a new file. I will call it `new_file.txt`
5. Run `git status again`
  * Now you can see something like `Untracked files: new_file.txt`
  * This means that git is aware of your change but it's not tracking it. Meaning that it won't capture your changes over time unless you tell it to.
6. Run `git add new_file.txt` to order git to track the file.
7. Run 'git status'
  * Now you can see `Changes to be committed:` and `new file: new_file.txt`. This is the staging area.
  * `The Staging Area` is where git tells that it is aware `new_file.txt` it's a new file and it is ready to be commited.
8. Now run `git commit -m “Adds new file"`
  *  `git commit` captures a snapshot of the files you added to track. Meaning that it will pin point the exact state of the files at this exact time.

Awesome! You have added your first commit. Now before proceeding try to add another commit: change a word in your file, add it to the staged area and commit your new change.

### Go to the next section: History

* (If you are on github): go to the top left corner and change the branch to `history`
* (If you cloned this repo): run `git checkout history` in your terminal
