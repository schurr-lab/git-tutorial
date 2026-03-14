# 👋 Lab Git & GitHub Onboarding

Welcome! Before contributing to lab repositories, please complete this short Git & GitHub tutorial.

The **most important goal** is to learn how to keep your work safely backed up using GitHub.

A good habit is to **commit and push your code at the end of every work day**.

By the end of this tutorial, you will know how to:

- Create a GitHub account
- Clone a repository
- Edit files in a repository
- Commit changes
- Push changes to GitHub

Later you will typically create **your own repository for your projects** and use GitHub as a backup and version history.

Most students use **Mac + PyCharm**, but we start with the **command line workflow** because it works everywhere.

---

# What are Git and GitHub?

**Git** is a version control system. It tracks changes to files over time and allows you to return to earlier versions of your code.

Key ideas:

- A **repository** stores a project and its history.
- A **commit** records a snapshot of your changes.
- You can always go back to previous commits.

**GitHub** is a website that hosts Git repositories online.  
This allows you to:

- back up your code
- work across multiple computers
- collaborate with others

---

# Step 0 — Create a GitHub Account

1. Go to https://github.com  
2. Create an account using your academic email  
3. Send your **GitHub username** to the lab admin (currently Roey) so you can be added to the organization

---

# Step 1 — Complete the GitHub "Hello World" Tutorial

Before continuing, complete the official GitHub beginner tutorial:

https://docs.github.com/en/get-started/start-your-journey/hello-world

This tutorial introduces:

- repositories
- commits
- branches
- pull requests

Once you finish it, return here to continue.

---

# Step 1.5 — Opening a Terminal

Many commands in this tutorial are run in a **terminal** (also called a command line).

<details>
<summary><strong>Mac</strong></summary>

Press **Command + Space**, type **Terminal**, and press **Enter**.

Alternatively:

Finder → Applications → Utilities → Terminal

</details>

---

<details>
<summary><strong>Windows</strong></summary>

You can use **Command Prompt** or **PowerShell**.

Option 1 — Command Prompt

1. Click the Start Menu
2. Type **cmd**
3. Open **Command Prompt**

Option 2 — PowerShell

1. Click the Start Menu
2. Type **PowerShell**
3. Open **Windows PowerShell**

After installing Git, you may also use **Git Bash**.

</details>

---

# Step 2 — Check Whether Git Is Already Installed

On some lab computers Git may already be installed.

Run:

```bash
git --version
```

If you see something like:

```
git version 2.x.x
```

Git is already installed.

If not, install it in the next step.

---

# Step 3 — Install Git

<details>
<summary><strong>Mac</strong></summary>

Run:

```bash
git --version
```

macOS will prompt you to install Command Line Tools.

</details>

---

<details>
<summary><strong>Windows</strong></summary>

Install Git:

https://git-scm.com/downloads

Then open **Git Bash** and verify:

```bash
git --version
```

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

Choose where you want to store your projects.

Navigate there:

```bash
cd path/to/your/projects
```

Clone the repository:

```bash
git clone https://github.com/schurr-lab/git-tutorial.git
cd git-tutorial
```

---

# GitHub Sign-In

Git may open a **GitHub login window** in your browser.

Choose:

**Sign in with your browser**

If you use **two-factor authentication**, enter the code from your authenticator app.

If a page asks you to authorize the **Git Ecosystem**, click it and confirm.

---

# After Cloning

You should see:

```
git-tutorial/
├── README.md
├── students.md
└── practice/
```

Enter the repository:

```bash
cd git-tutorial
```

---

# Step 6 — Edit the File `students.md`

Open the file:

```
students.md
```

You can use **any text editor**, for example:

- PyCharm
- VS Code
- Notepad
- TextEdit

Add your name:

```markdown
- Alice Smith – PhD Student – 2026
```

Save the file.

---

# Step 7 — Practice Task

Inside the `practice/` folder create a file:

```
yourname.txt
```

Example:

```
alice-smith.txt
```

Write:

```
Hello GitHub!
This is my first Git commit.
```

Save the file.

---

# Step 8 — Commit Your Changes

```bash
git add students.md practice/yourname.txt
git commit -m "Add Alice Smith to students list and practice file"
```

A **commit** records your changes.

---

# Step 9 — Push Your Changes to GitHub

```bash
git push
```

This uploads your changes to GitHub.

Now your work is safely stored online.

---

# Daily Workflow (Most Important Habit)

When working on your own projects:

1. Edit your files
2. Save them
3. Commit your work

```
git add .
git commit -m "Describe what you did"
git push
```

Doing this **at the end of every day** ensures your code is always backed up.

---

# Appendix — Using PyCharm Instead of the Terminal

If you prefer PyCharm:

https://www.jetbrains.com/help/pycharm/set-up-a-git-repository.html

Typical workflow:

1. **Clone repository**

File → Get from VCS

2. **Edit files**

3. **Commit**

Use the **Commit** tab.

4. **Push**

Click **Push**.

---

# Advanced Topics (Optional)

These features are important when **collaborating on shared repositories**.

### Branches

Branches allow you to work on changes without affecting the main project.

Example:

```
git checkout -b new-feature
```

### Pull Requests

A **Pull Request** asks maintainers to review and merge your changes.

This is commonly used when multiple researchers collaborate on the same codebase.

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

Lab administrators review and maintain this repository.

If you encounter problems, open a **GitHub issue** or ask a lab member.
