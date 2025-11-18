# Understanding Basic Git Commands

Git is a distributed version control system that helps developers track changes in their codebase and collaborate efficiently.  
Here’s a beginner-friendly explanation of some of the most essential Git commands — perfect for a 15-minute talk!

---

## 1. git init  
**Purpose:** Initializes a new Git repository in your project folder.  
**Example:**  
You use this when starting a new project that you want to track with Git.  
It creates a hidden `.git` folder that stores all version control data.  

*Example workflow:*  
You create a folder for your project and initialize Git to start tracking files.

---

## 2. git add  
**Purpose:** Moves your file changes to the *staging area*.  
Think of the staging area as a “waiting room” for files you want to commit.  

*Example:*  
You edited or added some files and now you’re preparing them for commit using `git add filename` or `git add .` (to add all files).

---

## 3. git commit  
**Purpose:** Takes everything from the staging area and saves it permanently in Git’s history.  
Each commit is like a *snapshot* of your project at that moment.  

*Example:*  
After adding your files, you commit with a message explaining what you changed.  
A good message might be: “Added homepage layout.”

---

## 4. git status  
**Purpose:** Shows the current state of your working directory and staging area.  
It tells you which files are modified, staged, or untracked.  

*Example:*  
You can run `git status` anytime to see what changes are waiting to be added or committed.

---

## 5. git log  
**Purpose:** Displays the history of commits made in the repository.  
You can see who made changes, when, and what the commit messages were.  

*Example:*  
You can use `git log` to review your project’s history or identify older versions of your code.

---

## 6. git branch  
**Purpose:** Lists all branches in your repository or creates a new one.  
Branches allow you to work on different features or fixes without affecting the main code.  

*Example:*  
You can create a new branch named *feature1* using `git branch feature1`.  
To see all branches, just run `git branch`.

---

## 7. git checkout  
**Purpose:** Switches between branches or restores files.  
When you move from one branch to another, Git changes your working directory to match that branch’s snapshot.  

*Example:*  
To switch to a branch named *feature1*, you’d use `git checkout feature1`.

---

## 8. git merge  
**Purpose:** Combines changes from one branch into another.  
Usually, you merge a feature branch into the main branch (*master* or *main*) after completing a task.  

*Example:*  
First, you switch to the main branch using `git checkout main`, then merge your feature branch: `git merge feature1`.

---

## Putting It All Together  

Here’s a simple workflow example you can follow:  

1. Create a new project folder.  
2. Initialize Git using **git init**.  
3. Create a file `a.txt` and add it to staging using **git add a.txt**.  
4. Commit it with **git commit -m "Add a.txt"**.  
5. Create a new branch called **leaf** using **git branch leaf**.  
6. Switch to it using **git checkout leaf**.  
7. Add a new file `b.txt` and commit it.  
8. Go back to the main branch using **git checkout main**.  
9. Merge the branch using **git merge leaf**.  

---

## Key Concepts  

**Staging Area:**  
Where changes wait before being committed — like a “to-do” list for Git.  

**HEAD:**  
A pointer that represents your current location in Git history.  
It tells you which branch and commit you are currently on.

---

## Tip for Beginners  
- Use **git status** often — it keeps you informed about what’s happening.  
- Write meaningful commit messages to understand your progress later.  
- Branches are your best friends — use them to experiment safely.

---

### Conclusion  
Git helps you track, manage, and collaborate on code efficiently.  
Once you master these commands, you’ll be comfortable managing any project version control workflow.
