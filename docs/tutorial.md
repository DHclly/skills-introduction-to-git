How do you combine branches?
There are multiple strategies for organizing commits. Usually, all in the name of different styles of organization, transparency, and traceability. Let's introduce the most common.
组织提交有多种策略。通常，这一切都是以不同组织风格、透明度和可追溯性为名。让我们介绍最常见的。

Fast-forward merge: Move the new commits from the child branch onto the parent branch.
快进合并 ：将新提交从子分支迁移到父分支。

Merge commit: Apply the changes as a single new commit on the parent branch. Leave the child branch in the network for traceability.
合并提交 ：将这些变更作为父分支的单一新提交应用。为了可追溯性，将子分支留在网络中。

Squash merge: Collapse the commits from one branch into a single new commit on the other branch.
压缩合并 ：将一个分支的提交合并为另一个分支的单个新提交。


git branch --list

git checkout main

git merge --no-ff fix-incomplete-high-score -m "Fix high score tracker"


git log --all --graph --oneline

git branch --delete fix-incomplete-high-score