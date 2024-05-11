# GitHubCommands
Codecademy project
# Project 1 
Let’s practice some Git branching.

In this project, you’ll be using Git to make a 1-page website for your friend Kay’s birthday party.

index.html is written in HTML. Don’t be afraid! You won’t be asked to write any HTML from scratch. If you’re interested in learning HTML, check out Codecademy’s HTML course.

If you get stuck during this project or would like to see an experienced developer work through it, click “Get Unstuck“ to see a project walkthrough video.

## Tasks

 **From the terminal, list the Git branches.**

 **Kay wasn’t sure where she wanted to host the party, so you made several Git branches to explore different locations.**
   Some of the branches are no longer needed. Delete the following branches:
   - moma
   - whitney

   You’ll need the `-D` option, because these feature branches were never merged into master:
git branch -D branchname

vbnet
Copy code

 **Kay wants to see a version of the webpage that includes an unordered list with bullet points instead of a paragraph to show information about the party.**
- Create a new branch called unordered-list and switch over to it.

 **In index.html, replace:**
```html
<p>Description: Join Kay in celebrating their 29th birthday with free food and beverages, karaoke and a special appearance by Willy Nelson. Also, feel free to explore the Met museum before or after you stop by! Presents for Kay optional.</p>
with this unordered list:

html

<ul>
    <li>Join Kay in celebrating their 29th birthday with free food and beverages</li>
    <li>karaoke and a special appearance by Willy Nelson</li>
    <li>explore the Met museum before or after you stop by!</li>
    <li>Birthday presents optional</li>
</ul>
```
Click Save.

Add index.html to the staging area.

Now make a commit.

Kay approves the changes you made in the unordered-list branch.

Switch over to master. Then, merge unordered-list into master. This will be a fast forward merge.
Kay wants the heading to be way bigger. Create a new branch called big-heading.

Now, switch over the big-heading branch.

To make the heading bigger, replace the line below:
html

<h1>Kay's Birthday Party</h1>
With this line:

html

<h1 style="font-size: 72px">Kay's Birthday Party</h1>
Then click Save.

Add index.html to the staging area.

Make a commit.

Kay approves of the giant heading!

Switch back over to the master branch. Then, merge big-heading into master.
sql

# Solution 
```
# Task 1: List Git branches
git branch

# Task 2: Delete branches
git branch -D moma
git branch -D whitney

# Task 3: Create and switch to the unordered-list branch
git checkout -b unordered-list

# Task 4: Replace paragraph with unordered list in index.html
# Replace the content of index.html manually or using a text editor

# Task 5: Add index.html to the staging area
git add index.html

# Task 6: Commit changes
git commit -m "Add unordered list to index.html"

# Task 7: Merge unordered-list into master
git checkout master
git merge unordered-list

# Task 8: Create and switch to the big-heading branch
git checkout -b big-heading

# Task 9: Replace heading with a bigger font size in index.html
# Replace the content of index.html manually or using a text editor

# Task 10: Add index.html to the staging area
git add index.html

# Task 11: Commit changes
git commit -m "Increase heading font size in index.html"

# Task 12: Merge big-heading into master
git checkout master
git merge big-heading

```
# ||||||------------------------------------------------------------------------------|||||
# Project 2
# Ruby Time Calculator

In this project, you’ll have to resolve merge conflicts in two markdown files. Markdown is a file format that converts easily into HTML. You won’t have to write any markdown, just identify the differences between lines.

Take a deep breath. You can do this!

If you get stuck during this project or would like to see an experienced developer work through it, click “Get Unstuck“ to see a project walkthrough video.

## Tasks

1. **You are currently on master.**
   Merge the edits branch into the master branch.
   This will create two merge conflicts: README.md and examples.md.

2. **Using the file navigator, open README.md and examples.md. Identify the merge conflicts.**

3. **In README.md, keep the file changes from the edits branch. Delete the file changes from HEAD.**
   Don’t forget to delete all of Git’s special markings that indicate a merge conflict.
   Click Save.

4. **Add README.md to the staging area.**

5. **Follow the same order of actions as above for examples.md: keep the edits branch file changes and delete the HEAD changes.**
   Click Save.

6. **Add examples.md to the staging area and make a commit. Your commit message could be “Resolve merge conflict”.**

7. **Delete the edits branch.**


# Solution 
```
# Task 1: Merge edits branch into master
git checkout master
git merge edits

# Task 2: Identify merge conflicts in README.md and examples.md (requires manual resolution)

# Task 3: Resolve merge conflict in README.md
# Open README.md file, keep changes from edits branch, delete changes from HEAD, save the file

# Task 4: Add README.md to staging area
git add README.md

# Task 5: Resolve merge conflict in examples.md
# Open examples.md file, keep changes from edits branch, delete changes from HEAD, save the file

# Task 6: Add examples.md to staging area and make a commit
git add examples.md
git commit -m "Resolve merge conflict"

# Task 7: Delete the edits branch
git branch -d edits

