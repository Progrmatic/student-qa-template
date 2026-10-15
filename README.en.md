# Student Q&A repo

[繁體中文](README.md) | **English**

This repository is empty: it is a template for working with your instructor. Follow the steps below to create **your own** repository from it, put your coursework in it, and ask questions and get code reviews there. Your repository is private: only you and the instructor can see it.

> **Please do not ask questions in this repository.** It is a template shared by every student; open issues in the repository you create.

## Create your own repository

### 1. Create your repository with "Use this template"

This repository is public, so you can start without waiting for any invitation. After you buy a course, GitHub may send you an invitation to join this repository; accepting or ignoring it makes no difference to the steps that follow.

At the top right of this repository's page, press **Use this template** → **Create a new repository**, then:

| Field | What to enter |
|---|---|
| Owner | Your own GitHub account |
| Repository name | Anything you like, such as the course's name |
| Visibility | **Private** (recommended) |
| Include all branches | Leave unchecked |

Press **Create repository** and you are done.

> **Please do not fork it.** A fork of a public repository is always public, so your coursework and questions would be visible to everyone, and the platform does not accept a fork of this repository. A repository made with "Use this template" can be private and is entirely yours.

### 2. Link your repository on the course page

1. Go back to the course page on Progrmatic and find the **GitHub Collaboration** section.
2. Paste the URL of the repository you just created, such as `https://github.com/your-account/repo-name`.
3. Press **Link & Install App**, which takes you to GitHub to install the course's GitHub App.
4. On GitHub, choose **Only select repositories**, select **only the repository you just created**, and save.
5. GitHub takes you back to the platform. The instructor joins your repository with write (push) access, usually within a few seconds.

### 3. Make sure Issues are on

The platform usually turns Issues on for you. If your repository has no **Issues** tab, go to **Settings → General → Features** and check **Issues**.

## Stuck? Open an issue

In your repository, go to **Issues → New issue** and pick a template. Each one comes in Chinese and in English; use the one in your language:

| Template | When to use it |
|---|---|
| **Question / Stuck** | You are stuck on an assignment, a test will not pass, or a piece of code makes no sense |
| **Code review request** | It works, and you would like the instructor to look at how it is written or designed |
| **Errata** | A video, a slide or the course's sample code has a typo, a mistake or something out of date |

The template walks you through what the instructor needs to know. A few tips:

- **One question per issue**, with the point in the title, such as "[Question] Knapsack: case 3 is off by one".
- **Paste error messages as text, not screenshots**, so the instructor can copy and search them. The template's fields format them for you; in a comment, wrap them in ```.
- **Say where the code is**: a branch, a commit, or a link to the lines (click a line number on GitHub to copy one).
- **Write down what you have already tried**, including what an AI told you. It shows the instructor where you are stuck.
- **Never paste passwords, tokens, API keys or personal data**, even though the repository is private.

Once the instructor replies, keep the conversation going in the issue, and close it when the problem is solved.

## Get a code review: open a pull request

The instructor can comment on your code line by line, which is far clearer than code pasted into an issue. The suggested flow:

```bash
# 1. Start a new branch from main
git switch main
git pull
git switch -c feat/your-assignment

# 2. Write code and commit
git add .
git commit -m "Say what this change does"

# 3. Push it to GitHub
git push -u origin feat/your-assignment
```

Then:

1. In your repository, GitHub offers the branch you just pushed: press **Compare & pull request**, with `main` as the base.
2. Follow the pull request template: what you did, and what you would like the instructor to look at.
3. Open an issue with the **Code review request** template and give the pull request's number, so the instructor knows it is ready.
4. When the instructor comments, keep committing and pushing to the same branch; the pull request updates by itself.

## FAQ

**The course page says the GitHub App cannot access my repository?**
The repository was not selected when the App was installed. Follow the course page's steps to the GitHub App settings, add the repository to the authorized list, and press **Re-link** on the course page.

**I want to use a different repository?**
You can change the linked repository in the course page's GitHub Collaboration section. The instructor leaves the old repository and joins the new one.

**A problem with the platform itself (the site, video playback)?**
Report it in the public [platform feedback repository](https://github.com/Progrmatic/progrmatic-feedback). It is public, so please do not post personal data or your code there.
