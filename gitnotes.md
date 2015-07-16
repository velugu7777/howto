##Create Repositories
Start a new repository
###How to init
	git init[project-name]
	Create a new local repository with the sepified name
###how to copy github file
	git clone[url]
	download a project and its entire version history
##Make changes
Review edits and commit files
###how to git add <file>
	git add file like jsnotes.md
###how to do git commit
	git commit -m ["message"]
###how to add git remote
	git remote add origin https:github.com/velugu7777/howto.git
###How to push
	git push -u origin master
###How to delete file
	rm -r file name
	rm -rf file name [force to delete]
	git rm -- catched [file name]
###How to see difference
	git diff
###How to display commit messages
	git log
	git log -p
###How to merge branches
			step1:see which branch you are in
			step2:any changes you done just save it
			step3:check git status
			step4:then now come to the git add .
			step5:after git commit -m "updated"
			step6:check status of branch
			step7:after which branch changes made on come out
			step8:after git checkout which branch you want to go
				ex:git checkout master it will be switched to branch
			step9:final step after this type git merge which branch to you want to merge
			 		ex:git merge gh-pages
			step10:git status
###	1.open github and create repository....username.github.io/projcet
		2.it will be serve the file index.html folder
		3.before that you have to create gh-pages branch in your project
		4.follow the instructions above mentiond..
