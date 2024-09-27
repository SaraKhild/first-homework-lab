# first-homework-lab

### 1. Set Up the Repository:
1.1 Create a new directory by mkdir task-manager<br>
1.2 Change into the cd taskmanager  directory<br>
1.3 Initialize a new Git repository  by git init<br>
1.4 Create a text file named tasks.txt by  touch tasks.txt<br>
	
### 2. Add Initial Tasks:
2.1 open file by open -e tasks.txt add this<br>
       - Learn Git basics<br>
			 - Set up Git repository<br>

2.2 Then add it to stage by  git add tasks.txt<br>		
2.3 dining commit for change  git commit -m "Add initial tasks to tasks.txt"<br>
2.4 for showing the commit by git log<br> 


### 3. Create Branches and Work on Features:
3.1 create and switch  new branch by git checkout -b feature/add-tasks<br>
3.2 create task  by echo "- Practice Git branching" >> tasks.txt<br>
3.3 add it to stage by git add tasks.txt<br>
3.4  doing commit by  git commit -m "Add task to feature add-tasks Git branching"<br>
3.5 to check out your commit git log<br> 
3.6 switch back to the main branch by git checkout main<br> 
3.7 create and switch  new branch by git checkout -b feature/remove-tasks<br>
3.8 open file and remove line then save it<br> 
3.9 add it to stage  by git add tasks.txt<br>
3.10 add commit by git commit -m "Remove a task from tasks.txt"<br>
3.11 to see commit by git log<br>
    
  
### 4. Merge Branches and Handle Conflicts:
4.1 switch back to the main branch by git checkout main<br> 
4.2 merge feature/add-tasks to main  by git merge feature/add-tasks<br>
4.3 then  merge  feature/remove-tasks to main  by git merge feature/remove-tasks<br>
4.4 there is conflict  in this merge so  open file by nano tasks.txt , solve it then save it <br>
4.5 add it to stage by git add tasks.txt<br>
4.6 add commit by  git commit -m "Resolve merge conflict in tasks.txt"<br>
4.7 to see commit by git log<br>


### 5. Use Git Rebase:
5.1 create and switch to new branch by git checkout -b feature/update-tasks<br>
5.2 add text to file by echo "- Review Git merge and rebase" >> tasks.txt<br>
5.3 add it to stage by git add tasks.txt<br>
5.4 add commit by  git commit -m "Add task to review Git merge and rebase"<br>
5.5 switch back to the main branch by git checkout main<br> 
5.6 rebase it by git rebase feature/update-tasks<br>


### 6. Reverting to Previous Commits:
6.1 echo "- Some incorrect task" >> tasks.txt<br>
6.2 git add tasks.txt<br>	
6.3 git commit -m "Add incorrect task"<br>	
6.4 git revert HEAD<br> 
6.5 git log to see   new commit  Revert "Revert "Add incorrect task""<br>

### 7. Working with Remote Repository:
a. Create a remote repository on GitHub.<br>
b. Link and push the local repository to the remote repository:<br>
	    git remote add origin <repository-url><br>
			Try to figure out the second command<br>		
	
echo "# first-homework-lab" >> README.md<br>
git init<br>
git add README.md<br>
git commit -m "first commit"<br>
git branch -M main<br>
git remote add origin https://github.com/SaraKhild/first-homework-lab.git<br>
git push -u origin main<br>
