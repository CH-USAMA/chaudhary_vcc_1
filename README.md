# chaudhary_vcc_1
VCC1 assignment - learning basic Git workflow
Here is a **complete dummy walkthrough** of the entire assignment using a fake student name **"chaudhary"** (so the repo name becomes `chaudhary_vcc_1`).  
Follow these steps **exactly** in order — copy-paste commands where possible. This matches the assignment requirements and follows the **Git best practices** from your slide (short, capitalized, no period, descriptive messages explaining **why**).

### Step 1: Create the repository on GitHub (do this in your browser)

1. Go to https://github.com/new
2. **Repository name**: `chaudhary_vcc_1` (all lowercase, exact spelling)
3. **Description**: VCC1 assignment - learning basic Git workflow
4. **Public** ← yes (toggle on)
5. Check these three boxes:
   - Add a README.md
   - Add .gitignore → choose "Node" or "None" (doesn't matter)
   - Choose a license → MIT License
6. Click **Create repository**

→ After creation you have **1 commit** (the initial one).

### Step 2: Clone locally (in terminal / Git Bash / PowerShell)

```bash
# Go to a folder where you want the project (example: Desktop)
cd ~/Desktop

# Clone (replace with YOUR github username if different)
git clone https://github.com/chaudhary/chaudhary_vcc_1.git

# Enter the folder
cd chaudhary_vcc_1
```

### Step 3: Create 5 new files

```bash
# Create empty files (or add content — both ok)
touch index.html
touch style.css
touch app.js
touch readme-notes.txt
touch data.txt

# Optional: put quick dummy content (makes it more realistic)
echo "<!DOCTYPE html><h1>Hello VCC World</h1>" > index.html
echo "body { font-family: Arial; background: #f0f0f0; }" > style.css
echo "console.log('App started');" > app.js
echo "These are my personal notes for the assignment." > readme-notes.txt
echo "Sample data line 1" > data.txt
```

### Step 4: First real commit + push (commit #2)

```bash
git add .
git commit -m "Add initial project files for basic webpage"
git push
```

→ Check GitHub → should now show **2 commits**

### Step 5: Make 3 modification cycles (each = edit → add → commit → push)

#### Modification 1 (commit #3)

```bash
# Edit one file
echo "<p>Added welcome paragraph - first change</p>" >> index.html

git add index.html
git commit -m "Update index.html with welcome message"
git push
```

#### Modification 2 (commit #4)

```bash
# Edit another file
echo "Added dark mode class" >> style.css
echo ".dark { background: #333; color: white; }" >> style.css

git add style.css
git commit -m "Add dark mode styling to CSS"
git push
```

#### Modification 3 (commit #5)

```bash
# Edit a third file (or same one again)
echo "// Added user greeting function" >> app.js
echo "function greetUser(name) { console.log('Hi ' + name); }" >> app.js

git add app.js
git commit -m "Implement greetUser function in app.js"
git push
```

→ After this → **at least 5 commits** total (initial + add files + 3 updates)

### Step 6: Show history and remote (exactly what teacher wants)

```bash
# Short pretty log
git log --oneline

# Show remotes
git remote -v
```

You should see something like this in terminal:

```
abcdefg Implement greetUser function in app.js
hijklmn Add dark mode styling to CSS
opqrstu Update index.html with welcome message
vwxyz12 Add initial project files for basic webpage
0000000 Initial commit (from README, .gitignore, LICENSE)
```

And remote:

```
origin  https://github.com/chaudhary/chaudhary_vcc_1.git (fetch)
origin  https://github.com/chaudhary/chaudhary_vcc_1.git (push)
```

### Step 7: Screenshot

- Take a screenshot of the **whole terminal output** showing both commands + results
- Crop if needed so both `git log --oneline` and `git remote -v` are clearly visible
- Save as **terminal.png** (exactly this name)

### Step 8: Submit in Teams

Send two things to your teacher (Michael Lewis):

1. Repo link:  
   `https://github.com/chaudhary/chaudhary_vcc_1`

2. Attach **terminal.png**

That's it — assignment complete.

### Quick summary of your commit messages (following best practices)

- Capitalized first letter
- No period at end
- Short (~30–50 chars)
- Descriptive (explains **what** and a bit of **why**)

Examples used:
- "Add initial project files for basic webpage"
- "Update index.html with welcome message"
- "Add dark mode styling to CSS"
- "Implement greetUser function in app.js"

You can use similar style — just change words to match what you actually did.

If you run into errors (e.g. authentication → use GitHub token or SSH), paste the error here and I'll help fix it quickly.

Good luck — you'll finish this in 10–15 minutes!