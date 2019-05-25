# simple-todos
Simple Todo app with meteor


## Startup
type `meteor`

(look this is a learning app, don't expect too much)

some things to note. I will be doing weird stuff with git.

If you want to create a git repos with the fully loaded git ignore but you already worked on your present repos
* create a new copy on your local called staging
* now your staging is an exact copy of your local master

Present Head-> local master
 8432  git checkout -b staging
  * so now i have a new staging branch
  * git add and commit all your changes
 8433  git pull --rebase origin master
  * rewind all your commits, fetch and merge all of master, then redo all your commits.
 8438  git push origin master (look, if you have to force it, do so, if your git log looks right, it looks right)
  * Your branch changes from staging to a `<hash>`
 8444  git branch -D  master
  * while sitting on `<hash>`delete your branch 
 8445  git checkout -b master
  * while sitting on `<hash>`, create a new branch called master (which will of course b a copy of your chair)
 8448  git push -f origin master
  * push the new master and overwrite the one above.

Never do this workflow on anything in production. This is just an exericse in git jumping jacks.
