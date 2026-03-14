# git-tutorial
A short tutorial for getting to know git and github

👋 Welcome to the Lab – Git & GitHub Onboarding

Welcome! Before contributing to lab repositories, please complete this short Git & GitHub tutorial.

By the end, you will:

Create a GitHub account

Clone a repository

Create a branch

Commit changes

Push to GitHub

Open a Pull Request

Modify files inside a practice/ folder

Most of you will use Mac + PyCharm, but command-line instructions are provided first because they work everywhere.

📌 Step 0 – Create a GitHub Account

Go to https://github.com

Create an account (use your academic email).

Send your GitHub username to the lab admin to be added to the organization.

💻 Step 1 – Install Git
🍎 Mac (most students)

Open Terminal and run:

git --version

If Git is not installed, macOS will prompt you to install Command Line Tools. Accept.

🪟 Windows

Install Git for Windows:
https://git-scm.com/downloads

Open Git Bash (recommended).

Verify installation:

git --version

We recommend using Git Bash so you can copy/paste commands exactly as written below.

🔐 Step 2 – Configure Git (First Time Only)

Run:

git config --global user.name "Your Name"
git config --global user.email "your@email.com"

Make sure this email matches your GitHub account.

📥 Step 3 – Clone This Repository
git clone https://github.com/YOUR-LAB-NAME/git-intro.git
cd git-intro
🌿 Step 4 – Create Your Own Branch

Create a branch using your name:

git checkout -b add-yourname

Example:

git checkout -b add-alice-smith
✏️ Step 5 – Add Yourself to students.md

Open students.md and add your name:

- Alice Smith – PhD Student – 2026

Save the file.

🧪 Step 6 – Complete the Practice Task

Go into the practice/ folder.

Create a new file named:

yourname.txt

Example:

alice-smith.txt

Inside the file, write:

Hello, GitHub!
This is my first branch and pull request.

Save the file.

💾 Step 7 – Commit Your Changes
git add students.md practice/yourname.txt
git commit -m "Add Alice Smith to students list and practice file"
🚀 Step 8 – Push to GitHub
git push origin add-yourname
🔁 Step 9 – Open a Pull Request

Go to the repository on GitHub.

Click Compare & pull request

Add a short description.

Click Create Pull Request

A lab admin will review and merge it.

🎉 Congratulations — you’ve completed your first Git workflow!

🧠 What You Just Practiced

Cloning a repo

Creating a branch

Editing files

Staging changes

Committing

Pushing

Opening a pull request

Code review workflow

This is the standard workflow used in the lab.

🧑‍💻 Appendix A – Using PyCharm Instead of Terminal

If you prefer PyCharm:

Clone

Open PyCharm

Select Get from VCS

Paste the repo URL

Clone

Create Branch

Bottom right → click current branch

New Branch

Name it add-yourname

Edit Files

Modify students.md

Create practice/yourname.txt

Commit

Open Commit tab

Select files

Write commit message

Click Commit and Push

Open Pull Request

Go to GitHub in your browser and create the PR.

⚠️ Important Lab Rules

Never push directly to main

Always create a branch

Always open a Pull Request

Keep commit messages clear and descriptive

🔥 Optional Challenge

Make a second commit improving your practice/ file

Edit this README and submit another PR

Add a markdown file instead of .txt
