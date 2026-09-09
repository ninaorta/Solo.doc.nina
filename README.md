# Solo.doc.nina

A beginner's guide to setting up a basic web-publishing workflow: an editor, a version-controlled repository, a live webpage, and a way to collaborate with others. You'll set these up once, but the core loop like *edit, commit, push*  repeats all semester, so it's worth understanding the flow.

## Before You Start: Navigating GitHub

GitHub's buttons move depending on what you're doing. **Commit changes** appears top-right when editing a file, at the bottom of the page when creating a new one, and disappears entirely when you're just viewing a file, there's nothing to save. **Repo-wide settings** (like Pages) live under the **Settings** tab; **file-level actions** (like adding a file) live inside the **Code** tab, near the file list. If a button seems missing, check which mode you're in before assuming something's broken.

## 1. Install an Editor

Install [Visual Studio Code](https://code.visualstudio.com/), then add the **Markdown All in One** extension for live preview and formatting shortcuts. This is where you'll write and edit files.

## 2. Get on GitHub

Create a free [GitHub account](https://github.com/join), then install [GitHub Desktop](https://desktop.github.com/). GitHub *hosts* your repo online; Desktop gives you buttons for Git actions instead of typing commands.

**Tip:** if Desktop can't find your local folder in VS Code, go to Desktop's **Integrations** settings and set VS Code as your external editor then use the **"Open in Visual Studio Code"** button instead of hunting for the folder yourself.

## 3. Create a Repository

Create a new **public** repository, public means anyone who has the link, including your professor, can view it without an account. Inside it, create a file named `index.html` containing a link back to the repo itself:

```html
<a href="https://github.com/ninaorta/Solo.doc.nina
```

## 4. Stage, Commit, Push

In GitHub Desktop: review your changed files (**stage**), write a short message describing what changed (**commit**), then click **Push origin** to upload. This habit keeps a readable history of your work instead of one long, unexplained blob of changes.

You can also edit files directly on github.com and click **Commit changes** — useful if your local setup is giving you trouble, though it skips practicing the local workflow you'll need all semester.

## 5. Deploy with GitHub Pages

In **Settings → Pages**, set the branch to `main` and save. Your live URL follows the pattern `username.github.io/repo-name/` — note the repo name is part of the URL. Just `username.github.io` alone won't work unless that's literally your repo's name.

## 6. Collaborate with a Pull Request

Add a collaborator under **Settings → Collaborators**. Have them edit a file and open a **pull request (PR)** — a proposed change you review *before* it merges.

**Tip:** adding a collaborator may trigger GitHub's "sudo mode," asking you to re-verify your identity by email first. This is a routine security check, not an error — click **Verify via email** and continue.

## 7. Write This File

Finally, create `README.md` at your repo's top level, and you're reading its contents now. A README is the first thing visitors see, so it's where you explain what a project *is* and *how to use it*. Save, commit, and push it like any other change. 
