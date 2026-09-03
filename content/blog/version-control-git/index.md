---
title: 'Version control and Git: how I stopped renaming folders'
summary: What Git actually does, which five commands cover most of my day, and why this site deploys itself.
date: 2026-08-06
authors:
  - me
tags:
  - Git
  - Tools
---

Before university my version control system was folders: `project`, `project_final`, `project_final2`, `project_final2_FIXED`. Everyone I know did this. It works until the day you need to remember what exactly changed between `final` and `final2`, and then it doesn't.

Git solves this properly. It keeps a full history of a project: every saved state, who made it, when, and with what comment. A saved state is called a commit. You can look at any old commit, compare two of them line by line, or roll the whole project back to last Tuesday.

In practice I use a small set of commands:

```bash
git status          # what changed
git add file.md     # stage the change
git commit -m "Add education section"
git push            # send commits to GitHub
git log --oneline   # history
```

That covers about 90 percent of my work. There are branches, merges and rebases underneath, and I understand them roughly at the level of "I read a tutorial once". For a personal website, the simple linear flow is enough.

GitHub is the second half of the story. Git itself is local; GitHub is a place to store the repository online. My repository is public, which felt uncomfortable at first, like leaving your notebook open on a desk. Then I realized nobody is reading it anyway, and if someone does, fine, the commit messages are decent.

The best part is what happens after `git push`. This site has a GitHub Actions workflow: every push to the main branch triggers a build, and a couple of minutes later the new version is live. I don't upload anything by hand. The first time it worked I pushed a typo fix just to watch the robot do its thing.

One habit I'm trying to build: commit messages that say why, not what. "Fix config" tells future me nothing. "Set baseURL so CSS loads on GitHub Pages" is a note from past me to future me. Past me is usually the only documentation I have.
