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

# 📚 Useful Resources

**Git tutorial**

https://git-scm.com/docs/gittutorial

**GitHub Hello World**

https://docs.github.com/en/get-started/quickstart/hello-world

**Install Git**

https://git-scm.com/downloads

**Markdown guide**

https://www.markdownguide.org/basic-syntax/

---

# Step 0 — Create a GitHub Account

1. Go to https://github.com  
2. Create an account using your academic email  
3. Send your **GitHub username** to the lab admin (currently Roey) so you can be added to the organization

---

# Step 1 — Install Git

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

# Step 2 — Configure Git (First Time Only)

Run:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

Make sure the email matches your GitHub account.

---

# Step 3 — Clone This Repository

First decide **where on your computer you want to store your projects**.

For example, many people keep code in a folder called `projects` or `repos`.

### Option A — Clone into the current folder

Navigate to the directory where you want the repository to live (use "/" or "\\" and not "\" as the latter will fail on Windows):

```bash
cd path/to/your/projects
```

Then clone the repository:

```bash
git clone https://github.com/schurr-lab/git-tutorial.git
cd git-tutorial
```

---

### Option B — Clone and specify the folder name

You can also tell Git exactly what folder to create:

```bash
git clone https://github.com/schurr-lab/git-tutorial.git my-git-practice
cd git-tutorial
```

This will create a directory called:

```
my-git-practice/
```

containing the repository.

---

After cloning, you should see something like this:

```
git-tutorial/
├── README.md
├── students.md
└── practice/
```

You are now ready to continue with the tutorial.


---

# Step 4 — Create Your Own Branch

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

# Step 5 — Add Yourself to `students.md`

Open the file:

```
students.md
```

Add your name at the bottom:

```markdown
- Alice Smith – PhD Student – 2026
```

Save the file.

---

# Step 6 — Practice Task

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

# Step 7 — Commit Your Changes

```bash
git add students.md practice/yourname.txt
git commit -m "Add Alice Smith to students list and practice file"
```

A **commit** records your changes.

---

# Step 8 — Push to GitHub

```bash
git push origin add-yourname
```

This uploads your branch to GitHub.

---

# Step 9 — Open a Pull Request

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

<details>
<summary><strong>PyCharm workflow</strong></summary>

### Clone repository

Open PyCharm → **Get from VCS**

Paste the repository URL and clone.

---

### Create a branch

Bottom right corner → click branch name → **New Branch**

Name it:

```
add-yourname
```

---

### Edit files

Modify:

```
students.md
practice/yourname.txt
```

---

### Commit

Open the **Commit** tab.

Select the files, write a commit message, then click:

```
Commit and Push
```

---

### Open Pull Request

Go to the repository page on GitHub and create the pull request.

</details>

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

# Maintainers

Lab administrators review and merge pull requests.

If you encounter problems, open a **GitHub issue** or ask a lab member.
