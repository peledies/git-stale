# git-stale
=========
Easily view old/stale branches sitting on the origin.

A Git extension for listing branches sorted by their last commit date in a column view with some color prettification

###Install instructions

### Install
```
  $ npm install git-stale -g
```

###Usage
From a current git project issue the following command
```
$ git stale
```

####Optional Argument
An optional argument can be added to git-stale to grep the output for matches. So if you wanted to only show branches created by a specific user then 
you could pass the users name, or if you wanted to search for a branch that had a certain text in its name you could pass that text.
```
$ git stale John
```