# 👋 Lab Git & GitHub Onboarding

Welcome! Before contributing to lab repositories, please complete this short Git & GitHub tutorial.

By the end, you will learn how to:

- Create a GitHub account
- Clone a repository
- Create a branch
- Commit changes
- Push to GitHub
- Open a Pull Request
- Modify files inside a practice folder

Most students use **Mac + PyCharm**, but we start with the **command line workflow** because it works everywhere.

---

# What are Git and GitHub?

**Git** is a version control system. It tracks changes to files over time and allows multiple people to collaborate on the same project without overwriting each other's work.

Key ideas in Git:

- A **repository** stores a project and its history.
- A **commit** records a snapshot of changes.
- A **branch** allows you to work on changes without affecting the main project.

**GitHub** is a cloud platform that hosts Git repositories and provides tools for collaboration such as pull requests, issue tracking, and code review.

---

# Step 0 — Create a GitHub Account

1. Go to https://github.com  
2. Create an account using your academic email  
3. Send your **GitHub username** to the lab admin (currently Roey) so you can be added to the organization

---

# Step 1 — Complete the GitHub "Hello World" Tutorial

Before continuing, complete the official GitHub beginner tutorial:

https://docs.github.com/en/get-started/start-your-journey/hello-world

This short tutorial will introduce:

- repositories
- commits
- branches
- pull requests

Once you finish it, return here to continue.

---

# Step 1.5 — Opening a Terminal

Many of the commands in this tutorial are run in a **terminal** (also called a command line or shell).

<details>
<summary><strong>Mac</strong></summary>

1. Press **Command + Space** to open Spotlight search  
2. Type **Terminal**  
3. Press **Enter**

Alternatively:

1. Open **Finder**
2. Go to **Applications → Utilities**
3. Open **Terminal**

A new window will appear where you can type commands.

</details>

---

<details>
<summary><strong>Windows</strong></summary>

You can use either **Command Prompt** or **PowerShell**.

### Option 1 — Command Prompt (simplest)

1. Click the **Start Menu**
2. Type **cmd**
3. Open **Command Prompt**

### Option 2 — PowerShell

1. Click the **Start Menu**
2. Type **PowerShell**
3. Open **Windows PowerShell**

A terminal window will appear where you can type commands.

After installing Git, you may also use **Git Bash**, which comes with Git for Windows and behaves more like a Linux/Mac terminal.

</details>

---

# Step 2 — Check Whether Git Is Already Installed

If you are working on a **lab computer**, Git may already be installed.

Open a terminal and run:

```bash
git --version
```

If Git is installed, you will see a version number such as:

```
git version 2.x.x
```

If the command fails, install Git as described below.

---

# Step 3 — Install Git

<details>
<summary><strong>Mac (most students)</strong></summary>

Open **Terminal** and run:

```bash
git --version
```

If Git is not installed, macOS will prompt you to install **Command Line Tools**. Accept.

</details>

---

<details>
<summary><strong>Windows</strong></summary>

1. Install **Git for Windows**

https://git-scm.com/downloads

2. Open **Git Bash** (recommended)

Verify installation:

```bash
git --version
```

Using **Git Bash** allows you to copy commands directly from this tutorial.

</details>

---

# Step 4 — Configure Git (First Time Only)

Run:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

Make sure the email matches your GitHub account.

---

# Step 5 — Clone This Repository

First decide **where on your computer you want to store your projects**.

Many people keep code in a folder called `projects` or `repos`.

Navigate there:

```bash
cd path/to/your/projects
```

Then clone the repository:

```bash
git clone https://github.com/schurr-lab/git-tutorial.git
cd git-tutorial
```

---

# GitHub Sign-In (Important)

When you run `git clone`, Git may open a **GitHub login window** in your browser.

This is normal. GitHub requires authentication when accessing organization repositories.

You will see two options:

- **Sign in with your browser (recommended)**
- **Use a Personal Access Token**

Choose **Sign in with your browser**.

---

# Two-Factor Authentication

If you have **two-factor authentication (2FA)** enabled on GitHub, you may be asked to verify your login.

Common methods include:

- GitHub mobile app
- Authenticator apps (Authy, Google Authenticator, etc.)

Open your authenticator app and enter the **6-digit code** when prompted.

---

# Important Note (Git Ecosystem Screen)

Some users see a page asking them to authorize the **Git Ecosystem**.

If this page appears:

1. Click **Git Ecosystem**
2. The **green confirmation button** will become enabled
3. Click the green button to continue

After authorization completes, the repository will finish cloning automatically.

---

# After Cloning

You should now see a new directory:

```
git-tutorial/
├── README.md
├── students.md
└── practice/
```

Enter the repository folder:

```bash
cd git-tutorial
```

You are now ready to continue the tutorial.

---

# Step 6 — Create Your Own Branch

Create a branch using your name:

```bash
git checkout -b add-yourname
```

Example:

```bash
git checkout -b add-alice-smith
```

Branches allow you to make changes without affecting the main project.

---

# Step 7 — Add Yourself to `students.md`

Open the file:

```
students.md
```

You can open it using **any text editor or IDE**, for example:

- PyCharm
- VS Code
- Notepad (Windows)
- TextEdit (Mac)
- or any editor you normally use

Navigate to the repository folder (`git-tutorial`) and open the file `students.md`.

Add your name at the bottom:

```markdown
- Alice Smith – PhD Student – 2026
```

Save the file after editing.

---

# Step 8 — Practice Task

Inside the `practice/` folder create a new file named:

```
yourname.txt
```

Example:

```
alice-smith.txt
```

Inside the file write:

```
Hello GitHub!
This is my first branch and pull request.
```

Save the file.

---

# Step 9 — Commit Your Changes

```bash
git add students.md practice/yourname.txt
git commit -m "Add Alice Smith to students list and practice file"
```

A **commit** records your changes.

---

# Step 10 — Push to GitHub

```bash
git push origin add-yourname
```

This uploads your branch to GitHub.

---

# Step 11 — Open a Pull Request

1. Go to the repository on GitHub  
2. Click **Compare & pull request**  
3. Add a short description  
4. Click **Create Pull Request**

A lab admin will review and merge it.

🎉 **Congratulations — you completed your first Git workflow!**

---

# What You Just Learned

You practiced:

- cloning a repository
- creating branches
- editing files
- committing changes
- pushing to GitHub
- creating pull requests

This is the **standard collaboration workflow used in the lab**.

---

# Appendix — Using PyCharm Instead of the Terminal

If you prefer using **PyCharm**, follow the official JetBrains guide:

https://www.jetbrains.com/help/pycharm/set-up-a-git-repository.html

Typical workflow in PyCharm:

1. **Clone repository**

   File → **Get from VCS**

2. **Create a branch**

   Bottom-right corner → branch name → **New Branch**

3. **Edit files**

   Modify:

   ```
   students.md
   practice/yourname.txt
   ```

4. **Commit and Push**

   Open the **Commit** tab → select files → **Commit and Push**

5. **Open Pull Request**

   Go to the repository page on GitHub and create the pull request.

---

# Lab Git Rules

Please follow these conventions:

- Always create a **branch** for changes
- Never push directly to **main**
- Use **pull requests** for merging
- Write **clear commit messages**

---

# Optional Challenge

Try one of the following:

- Improve your `practice/` file and make a second commit
- Edit this README and submit another pull request
- Add a Markdown file instead of `.txt`

---

# Repository Structure

```
git-tutorial/
│
├── README.md
├── students.md
├── practice/
│
└── .gitignore
```

---

# Additional Resources

Git tutorial  
https://git-scm.com/docs/gittutorial

GitHub documentation  
https://docs.github.com

Markdown guide  
https://www.markdownguide.org/basic-syntax/

---

# Maintainers

Lab administrators review and merge pull requests.

If you encounter problems, open a **GitHub issue** or ask a lab member.
