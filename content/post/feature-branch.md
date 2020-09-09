+++
author = "Pål"
title = "Feature branch workflow"
date = "2020-09-09"
description = "Feature branch git workflow utilizing github projects."
tags = [
    "Git",
]
categories = [
    "Technology"
]
series = ["Git"]
+++

Feature branch git workflow utilizing github projects.

<!--more-->

#### 1: Checkout master branch and update to latest version

```
git checkout master
git pull origin master
```

#### 2: Create your new feature branch

```
git checkout -b feature/GoodNameThatExplainsWtfIsBeingMadeInTheBranch
Branch name examples:
- feature/CreatePokemonView
- feature/AddPokemon
- feature/RemovePokemon
```

#### 3: Push feature branch to remote

```
git push -u origin feature/BranchName
```

#### 4: Create pull request to merge into master

This will create a card for your branch in the GitHub project under "in progress"

#### 5: Implement the feature

- Focus on implementing only one specific feature.
- Be cautious about not creating conflicts.
- If you feel like you have finished a part of your implementation, commit and push it to remote branch.

```
git status
git add filename
git commit filename
```

#### 6: Push feature branch to remote

```
git push -u origin feature/BranchName
```

#### 7: Merge pull request after receiving approvals
