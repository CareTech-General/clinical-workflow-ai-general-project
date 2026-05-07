# clinical-workflow-ai-general-project

## Repository Folder Structure

| `data/` | Stores datasets for the projects — will be added later in the quarter |

| `notebooks/` | Coding and model notebooks — this is where your actual project code goes |

| `docs/` | Plan and document your project in plain writing — start here before anything else |

| `workflow-diagrams/` | Upload visual maps of your clinical workflow — a diagram showing how your AI fits into a real hospital process |

| `presentations/` | 

## Getting started

### Step 1 - Fork & Clone the Repository

Click the **Fork** button at the top right of the repo page. This allows you to create own copy under you Github account

Then clone it to your computer:

Open **Terminal** (**Mac**)
Open **Command Prompt** (**Windows**)

```bash
# Replace YOUR-USERNAME with your actual GitHub username
git clone https://github.com/YOUR-USERNAME/clinicial-workflow-ai-general-project.git

# Navigate into the folder
cd clinicial-workflow-ai-general-project
```

### Step 2 — (Optional) Create a New Branch

If you want to keep different parts of your project separate, you can create a
branch. This is like making a separate workspace inside your fork.

```bash
git checkout -b your-branch-name
```

If you created a new branch, push it to GitHub right away:
```bash
git push origin your-branch-name
```

### Step 3 - Make, Test, and Save your Changes

Edit your files, then before saving make sure:
- Your notebook runs without errors (Restart & Run All in Jupyter)

Once you're happy with your changes, open your terminal and run these commands in order:

**Stage** — tell Git which files you want to save:
```bash
git add .
```

**Commit** — write a short note describing what you did:
```bash
git commit -m "your short description here"
```

Good commit message examples:
```bash
git commit -m "Add data exploration notebook for patient triage dataset"
git commit -m "Update project doc with AI inputs and outputs"
git commit -m "Upload current workflow diagram"
```

**Push** — upload your changes to GitHub:
```bash
git push
```

### Step 4 — Sync Your Fork With the Main Repo

If CareTech leads push updates to the main repo (such as new datasets or
templates), you'll want to pull in those changes without starting over.
Open your terminal and run:

---

#### Option A — Sync on GitHub Website (Easier)

1. Go to your forked repository on GitHub
2. Click the **"Sync fork"** button near the top of the page
3. Click **"Update branch"**

That's it! Your fork is now up to date. ✅

---

#### Option B — Sync via Terminal

**1. Add the main repo as "upstream" — only do this once:**
```bash
git remote add upstream https://github.com/CareTech-General/clinicial-workflow-ai-general-project.git
```

**2. Fetch the latest updates from the main repo:**
```bash
git fetch upstream
```

**3. Switch to your main branch:**
```bash
git checkout main
```

**4. Merge the updates into your copy:**
```bash
git merge upstream/main
```

**5. Push the synced changes to your fork:**
```bash
git push origin main
```
