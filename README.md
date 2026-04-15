# New Repository
commands for main branch creation:
====================================
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB$ cd ostad

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad$
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad$ mkdir newrepo

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad$ cd newrepo

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ ls

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git init

hint: Using 'master' as the name for the initial branch. This default branch name

hint: is subject to change. To configure the initial branch name to use in all

hint: of your new repositories, which will suppress this warning, call:

hint:

hint:   git config --global init.defaultBranch <name>

hint:

hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and

hint: 'development'. The just-created branch can be renamed via this command:

hint:

hint:   git branch -m <name>

Initialized empty Git repository in /mnt/c/Users/SHOEB/ostad/newrepo/.git/

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ echo "# New Repository" >> README.md

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git add README.md

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git commit -m "Initial commit to new repo"

[master (root-commit) 0dd7431] Initial commit to new repo

 1 file changed, 1 insertion(+)

 create mode 100644 README.md
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git remote add origin https://github.com/muhammadshoebalam/newre
po.git

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git branch -m main

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git push -u origin main

remote: Repository not found.

fatal: repository 'https://github.com/muhammadshoebalam/newrepo.git/' not found

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git push -u origin main

Enumerating objects: 3, done.

Counting objects: 100% (3/3), done.

Writing objects: 100% (3/3), 241 bytes | 24.00 KiB/s, done.

Total 3 (delta 0), reused 0 (delta 0), pack-reused 0

To https://github.com/muhammadshoebalam/newrepo.git

 * [new branch]      main -> main

branch 'main' set up to track 'origin/main'.

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ ls

README.md

=============END=============

##command for develop and feature branch
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git branch develop

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git switch develop

Switched to branch 'develop'

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git add .

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git switch main

Switched to branch 'main'

Your branch is up to date with 'origin/main'.

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ nano testfile.txt

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ ls

README.md  testfile.txt

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ cat testfile.txt

echo "New test file added."

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git add .

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git push origin main

Everything up-to-date

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git switch develop

A       testfile.txt

Switched to branch 'develop'

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ ls

README.md  testfile.txt

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ nano testfile.txt

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git add testfile.txt

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git commit -m "1st modification in develop branch"

[develop 40470ee] 1st modification in develop branch

 1 file changed, 2 insertions(+)

 create mode 100644 testfile.txt

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git push origin develop

Enumerating objects: 4, done.

Counting objects: 100% (4/4), done.

Delta compression using up to 16 threads

Compressing objects: 100% (3/3), done.

Writing objects: 100% (3/3), 362 bytes | 45.00 KiB/s, done.

Total 3 (delta 0), reused 0 (delta 0), pack-reused 0

remote:

remote: Create a pull request for 'develop' on GitHub by visiting:

remote:      https://github.com/muhammadshoebalam/newrepo/pull/new/develop

remote:

To https://github.com/muhammadshoebalam/newrepo.git

 * [new branch]      develop -> develop

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git checkout -b feature-featurebranch1

Switched to a new branch 'feature-featurebranch1'

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ nano testfile1.txt

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git add testfile1.txt

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git commit -m "new test file added in feature branch 1"

[feature-featurebranch1 d980ba6] new test file added in feature branch 1

 1 file changed, 1 insertion(+)

 create mode 100644 testfile1.txt

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git push origin feature-featurebranch1

Enumerating objects: 4, done.

Counting objects: 100% (4/4), done.

Delta compression using up to 16 threads

Compressing objects: 100% (2/2), done.

Writing objects: 100% (3/3), 373 bytes | 2.00 KiB/s, done.

Total 3 (delta 0), reused 0 (delta 0), pack-reused 0

remote:

remote: Create a pull request for 'feature-featurebranch1' on GitHub by visiting:

remote:      https://github.com/muhammadshoebalam/newrepo/pull/new/feature-featurebranch1

remote:

To https://github.com/muhammadshoebalam/newrepo.git

 * [new branch]      feature-featurebranch1 -> feature-featurebranch1

shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ ls

README.md  testfile.txt  testfile1.txt

================End==================
