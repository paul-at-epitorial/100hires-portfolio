# Environment Setup – 100Hires Portfolio

## A. TOOLS TO INSTALL

- Cursor
- Claude Code
- Codex

## B. STEPS TO TAKE

### B1. Setting Up Cursor

1. Download and install Cursor. Go to this website to begin: https://cursor.com/
2. Open the downloaded file and run it.
3. Accept the agreement and then just click `Next` a few times after that.
4. On one screen, you may be shown some options like creating a desktop icon, adding `Open with Cursor` action to Windows Explorer file context menu, so on. Check that applies. What those options mean:

	a) `Create a desktop icon` – Adds a Cursor shortcut on the desktop so you can open it quickly

	b) `Add “Open with Cursor” action to Windows Explorer file context menu` – Lets you right-click a file and open that file directly in Cursor

	c) `Add “Open with Cursor” action to Windows Explorer directory context menu` – This one lets you right-click a folder and open the whole folder/project in Cursor

	d) `Register Cursor as an editor for supported file types` – Allows Windows to recognize Cursor as an editor for code-related files it supports.

	e) `Add to PATH` – Enables you to open Cursor from the terminal or command prompt using a command (this may require restarting the shell or terminal before it works)

5. Click `Install` to start the installation. This may take a few minutes.
6. Once done, click `Finish` and launch Cursor.
7. Sign up if you haven’t yet then log in.
8. Make sure to connect GitHub. This will be used in the later instructions.
9. If not done yet, install and authorize Cursor.
10. Go back to the Cursor app. Click `Continue.` Wait for it to finish loading.
11. Cursor stuck at `Loading...`? Try to close out of it and run it again. Repeat the previous step.
12. Tick the box that’s shown to proceed.

### B2. Installing Claude Code

1. From the menu up top, click `View` and select `Extensions`.
2. A list of extensions will appear on the left sidebar. Click that rectangular box and search for *Claude Code for VS Code*.
3. Select the first one that appears and then click `Install`. Press `Trust Publisher & Install` to continue.
4. When it’s done installing, a dialog may pop-up, requesting your permission to allow access.
5. Now, click that down arrowhead symbol on the left sidebar. Choose `Claude Code`.
6. There will be a screen showing you how you want to log in. Click `Claude.ai Subscription`.
7. Some dialog will pop-up asking if you want Cursor to open the external website. Choose first `Configure Trusted Domains` so that you won’t be asked this again later. Select the second option (`Trust claude.com and all its subdomains`). Then, it will open a tab in your browser. Go ahead and log in from there.
Need to subscribe first before using? Check out the solution at the bottom.

### B3. Configuring Codex Access

1. Next up is installing Codex. Please repeat the same steps we did for Claude Code. Just see to it that `Sign in with ChatGPT` is selected when you log in.
2. You’re all set for Cursor. But don’t close it yet! We’re going to need it to set up the GitHub repository.

### B4. Finalizing via GitHub

1. Log in to GitHub: https://github.com/
2. In the top-right corner, click the `+` icon and select `New repository`.
3. Name the repository, for example, *100hires-portfolio*.
4. Keep it set to public. Leave the repository completely empty. **Important:** Do not toggle `Add a README file` since we’ll be creating our own README.
5. Click `Create repository`.
6. Keep the next page open -- you will need the repository URL (it looks like https://github.com/YOUR_USERNAME_GOES_HERE/100hires-portfolio.git).
7. On your desktop screen, create a new empty folder and name it *100hires-portfolio*.
8. Head back to Cursor.
9. Click `File` → `Open Folder...` and select the empty folder you just created.
10. In Cursor’s left sidebar, hover your cursor on it and then click the New File icon that appears. Name it README.md and press Enter.
11. Paste everything you just wrote for these instructions into the file (the blank space in the middle) and save it (shortcut: `Ctrl` + `S` or `Cmd` + `S`).
12. Open Cursor’s built-in terminal by pressing `Ctrl` + `~` (press `Control` and the tilde keys) at the same time or selecting `View` → `Terminal` from the top menu.
13. In the terminal, click inside it and run the following git commands one by one. Press **Enter** after each. **Note:** Ignore and close that small pop-up on the lower left telling you something about keybindings.

```
	git init

```

- **Purpose:** It initializes the local directory as a Git repository.

---

```
	git add README.md

```

- **Purpose:** Stages your new README file.

---

```
	git commit -m "first commit"

```

- **Purpose:** Saves the file with a note attached indicating the changes you’ve made.

---

```
	git branch -M main

```

- **Purpose:** Sets the main branch name.

14. Link your local folder to the GitHub repository you created earlier. Replace the URL below with your actual repository URL and run this command:

```
	git remote add origin https://github.com/YOUR_USERNAME_GOES_HERE/100hires-portfolio.git
```

15. Then push the code to GitHub:
```
	git push -u origin main
```

- **Note:** This may be your first time using Git on this computer, so it may prompt you to log in to GitHub via a browser window to authenticate the push. Once the terminal says the push was successful, refresh your GitHub page to verify the README.md file is live.

16. Well done! You’re all set.

## C. ISSUES RAN INTO + SOLUTION

– Cursor stuck at the `Loading...` screen. A simple close-and-run-again method will fix it.

– Different Claude Code extensions (clones) are available in the Marketplace. Select the one that has a publisher named *Anthropic (anthropic.com)* with a verified badge.

– Claude Code requires Claude Max or Pro subscription. If you don’t want to subscribe to a $20 monthly plan, use the Claude Console (https://platform.claude.com/login?returnTo=%2F%3F) to go around it. It’s only $5 one-off at the minimum to get access.

– Want to make changes to your README file and save it to GitHub? To do that, check first that your Cursor’s terminal is open. Just remember to run these three commands next time one by one, pressing Enter after each:

```
	git add README.md
	
	git commit -m "INSERT_A_SHORT_NOTE_THAT_DESCRIBES_YOUR_CHANGES"
	
	git push
```

Since you already linked the repository and pushed your initial setup, you do not need the longer setup commands from earlier. The basic git push will recognize the link and upload the newest version of your file.

– “*I don’t see the changes made to the README file on GitHub.*” Did you hit save (`Ctrl` + `S`) on the file from Cursor? A white circle appearing beside the filename means that you have unsaved changes.