A. TOOLS TO INSTALL

Cursor
Claude Code
Codex

B. STEPS TO TAKE

B1. Setting Up Cursor

1. Download and install Cursor. Go to this website to begin: https://cursor.com/
2. Open the downloaded file and run it.
3. Accept the agreement and then just click "Next" a few times after that.
4. In one screen, you may be shown some options like creating a desktop icon, adding “Open with Cursor” action to Windows Explorer file context menu, so on. Check that applies. What those options mean:

a) Create a desktop icon – Adds a Cursor shortcut on the desktop so you can open it quickly
b) Add “Open with Cursor” action to Windows Explorer file context menu – Lets you right-click a file and open that file directly in Cursor
c) Add “Open with Cursor” action to Windows Explorer directory context menu – This one lets you right-click a folder and open the whole folder/project in Cursor
d) Register Cursor as an editor for supported file types – Allows Windows to recognize Cursor as an editor for code-related files it supports.
e) Add to PATH – Enables you to open Cursor from the terminal or command prompt using a command (this may require restarting the shell or terminal before it works)

5. Click "Install" to start the installation. This may take a few minutes.
6. Once done, click "Finish" and launch Cursor.
Sign up if you haven’t yet then log in.
Make sure to connect GitHub.
If not done yet, install and authorize Cursor.
Go back to the Cursor app. Click “Continue.” Wait for it to finish loading.
Cursor stuck at “Loading...”? Try to close out of it and run it again. Do the same as the previous step.
Tick the box that’s shown to proceed.

B2. Installing Claude Code

From the menu up top, click "View" and select "Extensions."
A list of extensions will appear on the left sidebar. Click that rectangular box and search for Claude Code for VS Code.
Select the first one that appears and then click "Install." Press "Trust Publisher & Install" to continue.
When it’s done installing, a dialog may pop-up, requesting your permission to allow access.
Now, click that down arrowhead symbol on the left sidebar. Choose Claude Code.
There will be a screen showing you how you want to log in. Click "Claude.ai Subscription."
Some dialog will pop-up asking if you want Cursor to open the external website. Choose first "Configure Trusted Domains" so that you won’t be asked this again later. Select the second option (“Trust claude.com and all its subdomains”). Then, it will open a tab in your browser. Go ahead and log in from there.
Need to subscribe first before using? Check out the solution below.

B3. Configuring Codex Access

Next up, installing Codex. Please repeat the same steps we did for Claude Code. Just see to it that "Sign in with ChatGPT" is selected when you log in.
You’re all set for Cursor. But don’t close it yet! We’re going to need to set up the GitHub repository.

B4. Finalizing via GitHub

Log in to GitHub: https://github.com/
In the top-right corner, click the + icon and select “New repository.”
Name the repository, for example, “100hires-portfolio.”
Keep it set to public. Important: Do not check “Add a README file.” Leave the repository completely empty.
Click “Create repository.”
Keep the next page open -- you will need the repository URL (it looks like https://github.com/YOUR_USERNAME_GOES_HERE/100hires-portfolio.git).
On your desktop screen, create a new empty folder and name it 100hires-portfolio.
Head back to Cursor.
Click “File” > “Open Folder...” and select the empty folder you just created.
In Cursor’s left sidebar, hover your cursor on it and then click the New File icon that appears. Name it README.md and press Enter.
Paste everything you just wrote for these instructions into the file and save it (shorcut: Ctrl + S or Cmd + S).
Open Cursor’s built-in terminal by pressing Ctrl + ~ (press Control and the tilde keys) at the same time or selecting “Terminal” → “New Terminal” from the top menu.
In the terminal, run the following commands one by one. Press Enter after each:

---

git init

Purpose: It initializes the local directory as a Git repository.

---

git add README.md

Purpose: Stages your new README file.

---

git commit -m "first commit"

Purpose: Saves the file with a note attached indicating the changes you’ve made.

---

git branch -M main

Purpose: Sets the main branch name.

---

Link your local folder to the GitHub repository you created earlier. Replace the URL below with your actual repository URL:

git remote add origin https://github.com/YOUR_USERNAME_GOES_HERE/100hires-portfolio.git

Then push the code to GitHub:

git push -u origin main

Note: This may be your first time using Git on this computer, so it may prompt you to log in to GitHub via a browser window to authenticate the push. Once the terminal says the push was successful, refresh your GitHub page to verify the README.md file is live.

C. ISSUES RAN INTO + SOLUTION

– Cursor stuck at the "Loading..." screen. A simple close-and-run-again method fixed it.
– Different Claude Code extensions (clones) are available in the Marketplace. Select the one that has a publisher named Anthropic (anthropic.com) with a verified badge.
– Claude Code requires Claude Max or Pro subscription. If you don’t want to subscribe to a $20 monthly plan, use the Claude Console (https://platform.claude.com/login?returnTo=%2F%3F) to go around it. It’s only $5 one-off at the minimum to get access.