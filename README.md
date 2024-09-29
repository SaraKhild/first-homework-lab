# first-homework-lab

### 1. Set Up the Repository:
1.1 Create a new directory by <mark>mkdir task-manager</mark><br>
1.2 Change into the <mark>cd taskmanager  directory</mark><br>
1.3 Initialize a new Git repository by <mark>git init</mark><br>
1.4 Create a text file named tasks.txt by <mark>touch tasks.txt<mark><br>
	
### 2. Add Initial Tasks:
2.1 open file by <mark>open -e tasks.txt</mark> add this<br>
       - Learn Git basics<br>
			 - Set up Git repository<br>

2.2 Then add it to stage by <mark>git add tasks.txt</mark><br>		
2.3 dining commit for change <mark>git commit -m "Add initial tasks to tasks.txt"</mark><br>
2.4 for showing the commit by <mark>git log</mark><br> 


### 3. Create Branches and Work on Features:
3.1 create and switch  new branch by <mark>git checkout -b feature/add-tasks</mark><br>
3.2 create task  by <mark>echo "- Practice Git branching" >> tasks.txt</mark><br>
3.3 add it to stage by <mark>git add tasks.txt</mark><br>
3.4  doing commit by  <mark>git commit -m "Add task to feature add-tasks Git branching"</mark><br>
3.5 to check out your commit <mark>git log</mark><br> 
3.6 switch back to the main branch by <mark>git checkout main</mark><br> 
3.7 create and switch  new branch by <mark>git checkout -b feature/remove-tasks</mark><br>
3.8 open file and <mark>remove line</mark> then <mark>save it</mark><br> 
3.9 add it to stage  by <mark>git add tasks.txt</mark><br>
3.10 add commit by <mark>git commit -m "Remove a task from tasks.txt"</mark><br>
3.11 to see commit by <mark>git log</mark><br>
    
  
### 4. Merge Branches and Handle Conflicts:
4.1 switch back to the main branch by <mark>git checkout main</mark><br> 
4.2 merge feature/add-tasks to main  by <mark>git merge feature/add-tasks</mark><br>
4.3 then  merge  feature/remove-tasks to main  by <mark>git merge feature/remove-tasks</mark><br>
4.4 there is conflict  in this merge so  open file by <mark>nano tasks.txt , solve it then save it </mark><br>
4.5 add it to stage by <mark>git add tasks.txt</mark><br>
4.6 add commit by  <mark>git commit -m "Resolve merge conflict in tasks.txt"</mark><br>
4.7 to see commit by <mark>git log</mark><br>


### 5. Use Git Rebase:
5.1 create and switch to new branch by <mark>git checkout -b feature/update-tasks</mark><br>
5.2 add text to file by <mark>echo "- Review Git merge and rebase" >> tasks.txt</mark><br>
5.3 add it to stage by <mark>git add tasks.txt</mark><br>
5.4 add commit by  <mark>git commit -m "Add task to review Git merge and rebase"</mark><br>
5.5 switch back to the main branch by<mark> git checkout main</mark><br> 
5.6 rebase it by <mark>git rebase feature/update-tasks</mark><br>


### 6. Reverting to Previous Commits:
6.1 <mark>echo "- Some incorrect task" >> tasks.txt</mark><br>
6.2 <mark>git add tasks.txt</mark><br>	
6.3 <mark>git commit -m "Add incorrect task"</mark><br>	
6.4 <mark>git revert HEAD</mark><br> 
6.5 <mark>git log to see   new commit  Revert "Revert "Add incorrect task""</mark><br>

### 7. Working with Remote Repository:
a. Create a remote repositoryon GitHub.<br>
b. Link and push the local repository to the remote repository:<br>
	    git remote add origin <repository-url><br>
			Try to figure out the second command<br>		
	
<mark>echo "# first-homework-lab" >> README.md<br>
git init<br>
git add README.md<br>
git commit -m "first commit"<br>
git branch -M main<br>
git remote add origin https://github.com/SaraKhild/first-homework-lab.git<br>
git push -u origin main<br></mark>
