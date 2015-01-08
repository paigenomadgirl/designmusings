## How to find out what directory you are in 

```
pwd
```

## How to enter the directory you should be in 

```
cd Desktop/designmusings/
```

### How to add a new post

```
hugo new blog/something_new.md
```

Change the drafts parameter to false for deploy

### How to run Debug Server

```
hugo server --theme=hugo-incorporated --watch --buildDrafts=true
```

### How to commit new post

Kill debug server before commit

To generate the static pages
```
hugo --theme=hugo-incorporated
```

To see changes
```shell
git status -s
```

To add changes 
```
git add -A .
```
To add chages to commit
```
git commit -m 'some commit message'
```

To send/push commit to github
```
git push
```

To deploy to heroku
```
git subtree push --prefix public heroku master
```

### What to do if Heroku says the Head is not uptodate???


Only need to run once to install
```
heroku plugins:install https://github.com/heroku/heroku-repo.git
```

To reset the heroku repo
```
heroku repo:reset -a designmusings
```

Once done, run the following to deploy to heroku
```
git subtree push --prefix public heroku master
```

BOOM!
