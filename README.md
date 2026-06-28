# git-assignment-2

## Setup

1. Fork this repository on GitHub.
2. Open VSCode, open a terminal, and clone **your fork**:
git clone <your-fork-url>
3. Change into the repository directory:
cd git-assignment-2
4. Open the `git-assignment-2` folder in VSCode.
5. Open the `README.md` file (this file). You will edit it in VSCode.
6. **Industry vocabulary**  
- **origin** = your fork (`your_username/git-assignment-2`)  
- **upstream** = my repository (`josephor1271/git-assignment-2`)

---

## Part 1 (Branching and merging within your fork)

1. Create a new branch named `writing`:
git checkout -b writing

2. Check which branch you are on: \
git status \
It should say you are on branch `writing`.

3. Push this branch to GitHub: \
git push -u origin writing

4. Make a change to the line below in this file: \
Rock Ridge high + ChemE

5. Add, commit, and push your changes: \
git add README.md \
git commit -m "Add school and intended major" \
git push

6. On GitHub, open a pull request **within your fork**:
- From: `writing`
- To: `main`
- Make sure you are **not** pull requesting upstream (my repository).  
  My username should not appear anywhere in the pull request.
- It should look like: `main <- writing`

7. Merge the pull request on GitHub.  
(If GitHub does not let you merge, you likely pull requested upstream by mistake.)

8. After merging, your `main` branch and your `writing` branch on GitHub should look identical.

9. You have now successfully used a branch and merged it into `main`.

---

## Part 2 (Making a pull request to my repository)

1. GitHub now has your merged changes, but your **local** repository does not yet. \
Switch to `main` locally: \
git checkout main

2. Make sure you are on `main`: \
git status

3. Pull the latest changes from GitHub: \
git pull

4. Add a new line below: \
WRITE A CONTROVERSIAL OPINION YOU HAVE HERE

5. Add, commit, and push your changes:
  - git add README.md
  - git commit -m "Add controversial opinion"
  - git push

6. Confirm that your controversial statement appears on the `main` branch of **your fork** on GitHub.

7. On GitHub, go to **Pull Requests** and open a new pull request:
- From: `your_username/git-assignment-2` `main`
- To: `josephor1271/git-assignment-2` `main`
- It should look like:  
  `josephor1271/git-assignment-2 main <- your_username/git-assignment-2 main`

8. Submit the pull request.

9. After the due date, I will accept one of the submitted pull requests.

---

## Submission

Submit a link to your fork of this repository on Google Classroom.

---

## Optional Challenge (Fix a Typo Using a Branch)

This part is optional, but recommended if you finish early.

1. Make sure you are on the `main` branch: \
git status \
If not: \
git checkout main

2. Create a new branch called `typo-fix`: \
git checkout -b typo-fix

3. Find **any typo or wording you think could be improved** in this README and fix it.

4. Add, commit, and push your changes: \ 
git add README.md OR git add . \
git commit -m "Fix typo in README" \
git push -u origin typo-fix

5. On GitHub, open a pull request **from `typo-fix` to `main` within your fork**.  \
Do **not** include my repository in this pull request.

6. Merge the pull request.

7. After merging, your `main` branch and your `typo-fix` branch should be identical.

If you complete this, you have now practiced the full GitHub workflow twice: \
branch → commit → push → pull request → merge.
