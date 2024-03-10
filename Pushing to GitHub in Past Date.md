So if you want to commit something on Git in the past date, you simply use these commands that help you to do so.

```bash
git commit --amend --no-edit --date="Sat Feb 2 20:00:00 2024 -0600"
```

1. To make a commit in the past date, you just want to add your changes in the local repository by running `git add .`
2. Commit changes using `git commit -m "Your commit message"`.
3. Run this `git commit --amend --no-edit --date="Sat Jun 5 20:00:00 2021 -0600"` command after a commit to amend the last commit with the timestamp noted. The --no-edit will leave the message as-is.
4. Push changes to GitHub or whichever platform you use by running git push.

Make sure you have to change the date and time according to your preference. This will create a commit to the particular date in the past and you do not lose your GitHub streak.

Or just use the command <mark class="hltr-red">git commit --amend --no-edit --date="Sat Jun 5 20:00:00 2021 -0600</mark>" & => <mark class="hltr-red">git push --force</mark>

   