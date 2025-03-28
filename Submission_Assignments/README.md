## Final Assignment Submission Guide

Depending on the IDE you're using (Jupyter Notebook, PyCharm, Google Colab, etc.), the submission process will differ slightly. In all cases, however, to submit your final assignment for *Advanced Epidemiology II*, you will be working with a GitHub repository that I will provide.

Since most of you are likely using Jupyter Notebook, I’ll begin with that workflow:

### Submitting via Jupyter Notebook
If you want to run Git commands, there are two main ways to do this:

- Directly from **within a Jupyter Notebook**, or
- **Via the Terminal**, which you can open by clicking the "+" symbol and selecting "Terminal" under the "Other" section.

> **Note**: If you're running Git commands directly from a notebook cell, prefix them with an exclamation mark (`!`), like this:

```bash
!git clone xyz
```

First you need to fork the repository. "Forking" a repository means creating a personal copy of the original GitHub repo. You can freely make changes to your fork without affecting the original repository.

Once you've forked the repository and made changes you’ll need to:
- **Stage** your changes
- **Commit** them with a meaningful message
- **Push** them to your GitHub repository (or **pull**, depending on the direction of sync)

---

There are several ways to do this, but here's the approach I recommend for submitting your assignment. If you haven't created an account on GitHub yet, please do so:

1. Open the link to the repository:
   https://github.com/ariee-24/Advanced_Epi_II_2024-25

2. In the top right corner, click the **“Fork”** button.
3. This will create **your own copy** of the repository under your GitHub account.

Now you will **copy the repository to your local computer**.

4. Open your forked repository (under your GitHub username).
5. Click the green **"Code"** button and copy the **HTTPS URL**.
   It should look something like:
   https://github.com/yourusername/Advanced_Epi_II_2024-25.git
6. Open a new Jupyter Notebook and run separately:

```bash
!git clone https://github.com/yourusername/Advanced_Epi_II_2024-25.git
!cd Advanced_Epi_II_2024-25
```

After cloning the repository, you should see a new folder named `Advanced_Epi_II_2024-25 in your file manager on the left side of your Jupyter Notebook interface.

7. Click on the folder and navigate to the subfolder named `Submission_Assignments`
8. Inside that folder, create a new folder using the following format: `lastname(s)_firstname(s)`
9. Copy your assignment file into your personal folder. If your assignment consists of multiple files (e.g., one for each exercise), include all of them in this folder.

> At this point, you've added your files to the repository structure.

Now go back to your notebook and **commit your assignment** using the following command:

```bash
!git commit -m "Add final assignment for Lastnames Firstnames"
```

10. Go to your GitHub account: Click on your **profile picture** in the top-right corner and select **Settings**.
11. In the left-hand menu, scroll down to the very bottom and click **Developer settings**.
12. Then select **Personal access tokens** → **Tokens (classic)**. Click the button "**Generate new token (classic)**".
13. Enter a name for your token (e.g., `Git for Jupyter) and choose an expiration date (e.g., 90 days).
14. Under scopes, **check the box for**: `repo`(this gives you permission to access and modify repositories) and click "**Generate token**".

> Important: Copy your token immediately – you will only see it once!

15. Now go back to your Jupyter Notebook, open the terminal by opening a new tab via clicking `+` and selecting "Terminal".
16. **Push** your assignment with this (no `!` needed anymore):

```bash
git push origin main
```
The terminal will ask you for your username and password:

17. Enter your **GitHub username**.
18. For the password, **enter your personal access token**. You can simply copy and paste it.

> Don’t worry if nothing appears when you enter your token! When typing sensitive information like a password or your personal access token in the terminal, no characters will be shown – the cursor will stay still, and the input box will appear blank. Be assured: your token is being entered correctly.

19. Hit `Enter`.
20. Go to your forked repo on GitHub and click the "**Contribute**" button -> "**Open Pull Request**". Choose:
    - base repository: `username/Advanced_Epi_II_2024-25`
    - base branch: `main`
    - head repository: your fork
    - compare branch: `main`
21. Add a short description.
22. Click "Create Pull Request" and wait for my reply that it worked. You did it!

---

### Submitting via PyCharm

If you're working with PyCharm, you’ll be submitting your assignment directly via the GitHub website, not through the IDE itself. Here’s how to do it:

1. Open PyCharm.
2. In the left sidebar (Project view), **right-click** on your project folder.
3. Select "**Show in Explorer**" (on Windows) or "**Reveal in Finder**" (on macOS).
4. This will open the folder location in your file system.
5. Typically, your project will be inside the `PyCharmProjects folder on your computer.
6. On your computer, create a new folder named after you in this format: `lastname(s)_firstname(s)` and put your assignment file(s) into that folder.

Upload your assignment:

7. Go to the following GitHub repository: https://github.com/ariee-24/Advanced_Epi_II_2024-25
8. Fork the repository to your own GitHub account (click the "Fork" button in the top-right corner).
9. Once forked, navigate to the `Submission_Assignments` folder in your forked repository.
10. Click on "**Add file**" → "**Upload files**".
11. Upload your folder containing your assignment file(s).
12. Scroll down, write a short commit message like "Add final assignment for Lastname Firstname" and click "**Commit changes**". 
13. Go back to your forked repository on GitHub. You should see a highlighted message: "**This branch is X commits ahead of ariee-24:main**" → Click on "**Contribute**" → then "**Open pull request**".
14. In the pull request, double-check that you're comparing:
    - base repository: ariee-24/Advanced_Epi_II_2024-25
    - head repository: your fork
15. Add a short title like: "Final assignment submission – Lastname(s) Firstname(s)"
16. Click "Create pull request".

That’s it! Now you only have to wait for my reply.

---

### Submitting via Google Collab

Download your assignment file(s) and pick up at Step 6 under “Submitting via PyCharm.”
