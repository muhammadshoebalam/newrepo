# New Repository
commands for main branch creation:
====================================
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB$ cd ostad \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad$ \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad$ mkdir newrepo \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad$ cd newrepo \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ ls \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git init \n
hint: Using 'master' as the name for the initial branch. This default branch name \n
hint: is subject to change. To configure the initial branch name to use in all \n
hint: of your new repositories, which will suppress this warning, call: \n
hint: \n
hint:   git config --global init.defaultBranch <name> \n
hint: \n
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and \n
hint: 'development'. The just-created branch can be renamed via this command: \n
hint: \n
hint:   git branch -m <name> \n
Initialized empty Git repository in /mnt/c/Users/SHOEB/ostad/newrepo/.git/ \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ echo "# New Repository" >> README.md \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git add README.md \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git commit -m "Initial commit to new repo" \n
[master (root-commit) 0dd7431] Initial commit to new repo \n
 1 file changed, 1 insertion(+) \n
 create mode 100644 README.md \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git remote add origin https://github.com/muhammadshoebalam/newre
po.git \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git branch -m main \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git push -u origin main \n
remote: Repository not found. \n
fatal: repository 'https://github.com/muhammadshoebalam/newrepo.git/' not found \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ git push -u origin main \n
Enumerating objects: 3, done. \n
Counting objects: 100% (3/3), done. \n
Writing objects: 100% (3/3), 241 bytes | 24.00 KiB/s, done. \n
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 \n
To https://github.com/muhammadshoebalam/newrepo.git \n
 * [new branch]      main -> main \n
branch 'main' set up to track 'origin/main'. \n
shoeb@LAPTOP-P61S2J2C:/mnt/c/Users/SHOEB/ostad/newrepo$ ls \n
README.md \n
=============END============= \n\n
