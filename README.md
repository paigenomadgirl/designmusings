## How To Do Things - :)

### How to add a new post

hugo new blog/something_new.md

Change the drafts parameter to false for deploy

### How to run Debug Server

hugo server --theme=hugo-incorporated --watch --buildDrafts=true

### How to commit new post
git status -s // To see changes

git add -A . // To add changes 

git commit -m 'some commit message' // To add chages to 
commit

git push // to send/push commit to github

git subtree push --prefix public heroku master // to deploy to heroku

### What to do if Heroku says the Head is not uptodate???

heroku plugins:install https://github.com/heroku/heroku-repo.git // Only need to run once to install

heroku repo:reset -a designmusings // to reset the heroku repo

Once done, run 

<code>
git subtree push --prefix public heroku master // to deploy to heroku
</code>

again!