# Lab 4 Answers


Question 1: What did --global mean here? What would happen if you left it out?

Answer: The --global flag tells Git to apply your name and email settings across every single repository on your entire user account. If left out, the config would only apply locally to the current folder, meaning you would have to re-enter your identity details for every new project.

Question 2: What appeared in ls -a but not in ls? What is inside it?

Answer: The hidden .git directory appeared in ls -a but was hidden in the standard ls command.

Question 3: Roughly how many files and folders is Git offering to track? Does anything in that list look like something you did not write?

Answer: Git was only offering to track 1 file '.gitignore'.

Question 4: Compare this git status with the one from Question 3. What disappeared?

Answer: Identical

Question 5: .gitignore itself shows up as untracked. Should it be committed, or ignored too? Why?

Answer: The .gitignore file must be committed rather than ignored. Committing it ensures that the exclusion rules are saved permanently into the repository's history so that every other developer or TA who pulls the project inherits the exact same file-blocking parameters.

Question 6: README.md moved from one heading to another in the git status output. Which two? In the three-places model, what just happened to it?

Answer: It moved out of the "Untracked files" heading and directly into the "Changes to be committed" heading. In the three-places model, running git add moved the file snapshot out of my local Working Directory and locked it into the Staging Area (Index).

Question 7: What did Git print after the commit? How many files did it say changed?

Answer: Git printed out the root commit hash metadata, the branch label, and a short message tracking the changes. It stated that 2 files changed with a set number of code text insertions.

Question 8: What are the first seven characters of your commit called, and what are they for?

Answer: The first seven characters are known as the short commit hash (a truncated version of the full SHA-1 identifier). They serve as a permanent, unique serial number to track, reference, or roll back to that specific snapshot in the history pipeline.

Question 9: You now have two commits. Without looking it up: what are the four steps of the loop you just did twice?

Answer: The four core steps of the revision lifecycle loop are:
1. Edit (modify code or files in the working tree)
2. Status (inspect changes via git status)
3. Stage (queue files for saving using git add)
4. Commit (permanently lock in the snapshot using git commit -m)

Question 10: Why does this file get a special name and a special place, rather than being called notes.md like everything else?

Answer: The README.md file serves as the universal entrance storefront for digital code projects and must live in the root directory. Platforms like GitHub are hardcoded to automatically parse and render this specific file as the rich-text homepage when anyone opens the repository online.

Question 11: What did gh auth login do that means you will not be asked for a password when you push?

Answer: The authentication protocol generates and caches a secure, encrypted Personal Access Token locally on your system. This allows your machine to securely prove its identity to GitHub's remote API servers automatically on every sync, completely eliminating the need to type password credentials.

Question 12: Refresh the repository page on GitHub. What is showing on the front page, and why that file?

Answer: The formatted text content of README.md is rendered front-and-center on the homepage. GitHub automatically displays this file by default to instantly provide visitors and project collaborators with context and instructions about the codebase.

Question 13: Run git log --oneline again. Did pushing change your local history in any way?

Answer: No, pushing did not alter or change your local history tracking structure in any way. It simply uploaded an identical duplicate copy of your existing local commit blocks up to GitHub's remote servers, appending an origin/main pointer tag to mark the sync point.

Question 14: Your repository is private but your TAs can now read it. In your own words, what is the difference between a repository being private and a repository not existing on GitHub at all?

Answer: A private repository physically exists securely on GitHub's cloud servers, but its visibility is restricted exclusively to the account owner and specific invited collaborators. A repository that does not exist at all has no data backup anywhere on the cloud network and cannot be shared with anyone.
