# github-cheatsheet

echo "# github-cheatsheet" >> README.md

git init

git add README.md

git commit -m "first commit"

git branch -M main

git remote add origin https://github.com/blentz100/github-cheatsheet.git

git push -u origin main


# common problems when first using github

You try to push your code to your Github repo but you get this error:

```console
src refspec master does not match any
```

If you see this error, it's possible your local branch is named master and the remote is named main. You can run ```git status``` to see what your local branch name is. After you first iniatilize your local git repo, it's a good idea to change the branch name to main by typing ```git branch -M main```.

It's also a really good idea to change your default git configuration to always use ```main``` as the default branch name so you don't have to change it every time you make a new repo. You can do that by running ```$ git config --global init.defaultBranch main```. If that doesn't work for you, read this [article](https://www.seancdavis.com/blog/git-set-default-branch/)
