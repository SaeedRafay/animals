# HYF WEEK3: Git Exercise (Branch)  
  
## Commands in Git Bash  
  
** $ git clone git@github.com:SaeedRafay/animals.git **  
Cloning into 'animals'...  
kex_exchange_identification: read: Connection reset by peer  
Connection reset by 140.82.121.4 port 22  
fatal: Could not read from remote repository.  

Please make sure you have the correct access rights and the repository exists.  


** $ git clone https://github.com/SaeedRafay/animals.git **  
Cloning into 'animals'...  
warning: You appear to have cloned an empty repository.  
  
  
** $ cd animals **  
  
  
** $ git status **  
On branch master  
No commits yet  
nothing to commit (create/copy files and use "git add" to track)  
  
  
** $ touch zoo.txt **  
  
  
** $ echo "Lion" >> zoo.txt **  
  
  
** $ echo "Giraffe" >> zoo.txt **  
  
  
** $ echo "Elephant" >> zoo.txt **  
  
  
** $ cat zoo.txt **  
Lion  
Giraffe  
Elephant  
  
  
** $ git add . **  
warning: LF will be replaced by CRLF in zoo.txt.  
The file will have its original line endings in your working directory  
  
  
** $ git commit -m "Three important wild animals added to a newly created text file" **  
  
  
** $ git push **  
  
  
** $ git branch new-animals **  
  
  
** $ git checkout new-animals **  
Switched to branch 'new-animals'  
  
  
** $ touch pets.txt **  
  
  
** $ echo "Cats" >> pets.txt **  
  
  
** $ echo "Dogs" >> pets.txt **  
  
  
** $ echo "Goldfish" >> pets.txt **  
  
  
** $ echo "Zebra" >> zoo.txt **  
  
  
** $ echo "Reindeer" >> zoo.txt **  
  
  
** $ cat pets.txt **  
Cat  
Dog  
Goldfish  
  
  
** $ cat zoo.txt **  
Lion  
Giraffe  
Elephant  
Zebra  
Reindeer  
  

** $ git add . **  
warning: LF will be replaced by CRLF in zoo.txt.  
The file will have its original line endings in your working directory  
warning: LF will be replaced by CRLF in pets.txt.  
The file will have its original line endings in your working directory   
  

** $ git commit -m "Three popular pets added to a new text file and two wild animals added to existing zoo.txt file" **
  

** $ git push **  
fatal: The current branch new-animals has no upstream branch.  
To push the current branch and set the remote as upstream, use  
git push --set-upstream origin new-animals  
  

** $ git push --set-upstream origin new-animals **  
  

** $ git checkout master **  
Switched to branch 'master'  
Your branch is up to date with 'origin/master'.  


** $ git merge new-animals **  