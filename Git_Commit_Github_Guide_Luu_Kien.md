Git Commit Github Guide
    1. In folder source will commit, init a git
Open terminal:
git init remote add <link is created on  github website>
    2. Create folder origin <this operation only create folder on local>
use: git remote -v to check what have remote
    3. Add all file in this present folder to folder Origin to manager
use: git add .
    4. Check information git has created
	use:  git status
    5. Config for the first commit
use: git commit -m “fist commit”

show as below to config for the fist commit
git config --global user.email "you@example.com"
git config --global user.name "Your Name"

git config --global user.email "nguyenquangvuongnd@gmail.com"
git config --global user.name "luukien"

    6. check again
use: git commit -m "first commit"

Show below as below:
 7 files changed, 177 insertions(+)
 create mode 100644 CMakeLists.txt
 create mode 100644 Makefile
 create mode 100644 README.md
 create mode 100644 main/CMakeLists.txt
 create mode 100644 main/Kconfig.projbuild
 create mode 100644 main/component.mk
 create mode 100644 main/main.c

    7. Push all file to server (Option 1)
git push origin master

Option 2:
	1.cd ~/.ssh/  - Folder of system

2.git remote -v

3.ssh-keygen create public key

 Show as below:
Generating public/private rsa key pair.
Enter file in which to save the key (/home/vncssd/.ssh/id_rsa): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/vncssd/.ssh/id_rsa.
Your public key has been saved in /home/vncssd/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:VdwZZkQi6Qeiz9VF9acffVNP0hIevrLM+UivEYnmcl4 vncssd@vncssd
The key's randomart image is:
+---[RSA 2048]----+
|          .oo=X+.|
|        . oo.*++.|
|       . o.o .= *|
|      .  .o.o. *=|
|       oS.o.+ oo+|
|        oo o = .+|
|        . o E   .|
|         + o =   |
|          . o.o  |
+----[SHA256]-----+

	ls check keygen
	id_rsa  id_rsa.pub  known_hosts
	
	4.cat id_rsa.pub
	
	
	Comeback to Website Github to get SSH keys

	
Setting -> SSH and GPG keys -> New SSH key

Type into  Title and copy :
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQC+YykuV7+MqncWaLVuXBG5MmJxAy4Kt17hig7ZVi14lOkSaQ8kf9iqOBw8LGgnWsLYQX+DtEjOHoUGAPcH6i+wmgpQ1X1b0VkDOb3RyZ48DMY+xYMtUBYDHD2z+6JFYrhDFZ2JJUmbWzumhQRI4FEv8E6fFaVTfp4OWXTup2TMUNUeyVZWlbaCn1CyyZE48+dt+w64tlcB4tI15NAsV5OCyS3n5nMmKMMgBuJaL+EXQYouYkbjOanHvq024lwFxySzB7woufm5r2haoEujAKpM6jh1nh2j37E42dM20d5nIS4cUnt2L9pK1ps5Gzj1dDNZGkgeFd/SCakS6PR vncssd@vncssd

from Step 4



Return folder need commit and push all file by:

git push origin master 


Git to your PC

Use terminal git:

git clone git@github.com:nguyenquangvuong/WifiAPESPRESSIF.git
