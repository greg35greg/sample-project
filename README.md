# sample-project
edureka@master:~$ cd sample-project/
edureka@master:~/sample-project$ ls
css  fonts  img  index.html
edureka@master:~/sample-project$ git init
Initialized empty Git repository in /home/edureka/sample-project/.git/
edureka@master:~/sample-project$ git add .
edureka@master:~/sample-project$ git status
On branch master

Initial commit

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   css/site.css
	new file:   fonts/segoeuil.ttf
	new file:   img/cloneWhite.svg
	new file:   img/deployWhite.svg
	new file:   img/lightbulbWhite.svg
	new file:   img/stackWhite.svg
	new file:   img/successCloudNew.svg
	new file:   img/tweetThis.svg
	new file:   index.html

edureka@master:~/sample-project$ git remote add origin https://github.com/KartikeyaEdureka/sample-project.git
edureka@master:~/sample-project$ git commit -m "first commit"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'edureka@master.(none)')
edureka@master:~/sample-project$ git config --global user.email "kartikeya.sinha@edureka.co"
edureka@master:~/sample-project$ git config --global user.name "KartikeyaEdureka"
edureka@master:~/sample-project$ git commit -m "first commit"[master (root-commit) 8128c4c] first commit
 9 files changed, 198 insertions(+)
 create mode 100644 css/site.css
 create mode 100644 fonts/segoeuil.ttf
 create mode 100644 img/cloneWhite.svg
 create mode 100644 img/deployWhite.svg
 create mode 100644 img/lightbulbWhite.svg
 create mode 100644 img/stackWhite.svg
 create mode 100644 img/successCloudNew.svg
 create mode 100644 img/tweetThis.svg
 create mode 100644 index.html
edureka@master:~/sample-project$ git push -u origin master
Username for 'https://github.com': kartikeya.sinha@edureka.co
Password for 'https://kartikeya.sinha@edureka.co@github.com': 
Counting objects: 14, done.
Compressing objects: 100% (12/12), done.
Writing objects: 100% (14/14), 460.43 KiB | 0 bytes/s, done.
Total 14 (delta 0), reused 0 (delta 0)
To https://github.com/KartikeyaEdureka/sample-project.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
edureka@master:~/sample-project$ git branch feature
edureka@master:~/sample-project$ git checkout feature
Switched to branch 'feature'
edureka@master:~/sample-project$ touch abc.txt
edureka@master:~/sample-project$ git status
On branch feature
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	abc.txt

nothing added to commit but untracked files present (use "git add" to track)
edureka@master:~/sample-project$ git add .
edureka@master:~/sample-project$ git commit -m "feature"
[feature 4556885] feature
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 abc.txt
edureka@master:~/sample-project$ git push -u origin feature
Username for 'https://github.com': kartikeya.sinha@edureka.co
Password for 'https://kartikeya.sinha@edureka.co@github.com': 
Counting objects: 3, done.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 270 bytes | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/KartikeyaEdureka/sample-project.git
 * [new branch]      feature -> feature
Branch feature set up to track remote branch feature from origin.
edureka@master:~/sample-project$ git checkout master
Switched to branch 'master'
Your branch is up-to-date with 'origin/master'.
edureka@master:~/sample-project$ git merge feature
Updating 8128c4c..4556885
Fast-forward
 abc.txt | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 abc.txt
