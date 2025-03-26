## Final Assignment Submission Guide

To submit your final assignment for *Advanced Epidemiology II*, please follow the steps below carefully. You will be working with the GitHub repository provided:

**Repository Link**:  
https://github.com/ariee-24/Advanced_Epi_II_2024-25/tree/fad0ff20d41a3c88e0c14628a9ef779c946e91a4

We will be using the GitHub workflow that includes:
- Forking the repository
- Cloning your fork
- Creating a new folder for your assignment
- Committing and pushing your work
- Submitting a pull request (PR)

---

### Step 1: Fork the Repository

1. Open the link to the repository:
   https://github.com/ariee-24/Advanced_Epi_II_2024-25

2. In the top right corner, click the **“Fork”** button.
3. This will create **your own copy** of the repository under your GitHub account.

---

### Step 2: Clone Your Fork

Now you will **copy the repository to your local machine**.

1. Open your forked repository (under your GitHub username).
2. Click the green **"Code"** button and copy the **HTTPS URL**.
   It should look something like:
   https://github.com/yourusername/Advanced_Epi_II_2024-25.git
3. Open your terminal and run:
```bash
git clone https://github.com/yourusername/Advanced_Epi_II_2024-25.git
cd Advanced_Epi_II_2024-25
```

---

### Step 3: Create Your Assignment Folder

1. Inside the cloned repository, create a folder with the following naming convention: `lastnames_firstnames/`
2. Inside this folder, place your final assignment Jupyter Notebook (e.g., `final_assignment.ipynb`) and any additional files you want to submit.
3. Alternatively, you can create the folder manually or via terminal:
```bash
mkdir lastname_firstname
mv your_assignment.ipynb lastnames_firstnames/
```

---

### Step 4: Stage and Commit Your Changes

1. Check the changes via
```bash
git status
```
2. Add your folger and its contents
```bash
git add lastnames_firstnames/
```
3. Commit with a clear message
```bash
git commit -m "Add final assignment for Lastnanmes Firstnames"
```

---

### Step 5: Push to Your GitHub Fork
```bash
git push origin main
```

### Step 6: Create a Pull Request

1. Go to your forked repo on GitHub
2. Click the "Contribute" button -> "Open Pull Request"
3. Choose:
    - base repository: `username/Advanced_Epi_II_2024-25`
    - base branch: `main`
    - head repository: your fork
    - compare branch: `main`
4. Add a short description like:

> "Submitting final assignment - Lastnames Firstnames"

5. Click "Create Pull Request"
