# GitHubCommands
Codecademy project
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



