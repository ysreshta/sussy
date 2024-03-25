# sussy-things

softlink: --> ln -s
	-->  ln -s /home/masaladosa/folder1/filename softlinkname
	-->  ls -la
	-->  echo "hello world" > filename

hardlink: --> ln
	-->  /home/masaladosa/folder1/filename hardlinkname 
	-->  ls -la
	-->  basically for backup

USER ACCOUNT MANAGEMENT

*userMAKING* 
	--> useradd idli
	--> id idli
	--> gid is group id 
	or
--> useradd -g(grp name) -s(/bin/bash) -c(comment) -m(home dir(if yes then -d(which is a path))) -d idli 
eg: useradd -g Test -a /bin/bash -c "Description" -m -d home/idli idli

--> id idli


*userDELETE*
	--> userdel idli
	--> userdel -r   (will remove HOME DIRectory)
	--> userdel -f   (FORCE del even if user is logged in)

*MODIFYuser*
	^for NEW grp but default grp will remain same --> usermod -G 
	eg: usermod -G Test idli
	
	^DEFAUL HI CHANGE KARNA HAI THEN --> usermod -g 

--> passwd idli 
su - idli


--> groupadd TEST
--> groupdel TEST
--> less /etc/passwd
/etc/shadow --> passwords 
