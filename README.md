# test-module
Sample to demo assignments, files, and workflow

# New Here? 
Just added the class? Remember to ask to join the `students` team. Also make sure to have the following software installed:  
- [R][download-r] Statistical Programming Language
- [RStudio][download-rstudio] Integrated Development Environment
- [git][download-git] for version control
- [TeX distribution][download-tex] for creating documents

# Explorations
These assignments are designed to enable engagement and practice with the concepts of applied statistics. 

### Git and github
Register for a github account and get comfortable with using git. [What is git/github][git-tour]? If you're having some trouble understanding or using git, read [this **presentation** from a UIUC stat student][coatless-presentation]. 

### RMarkdown
Your code should be readable and reproducible. We recommend using [RMarkdown][markdown-lessons] so that you can add comments, clarifications, and codechunks directly into the assignments. You should be able to knit assignments to pdf or html -- try it. If it does not work, troubleshoot.  

### To manually turn in your assignment: 
1. To start, [**fork** the repository][forking].
1. [**Clone**][ref-clone] the repository to your computer.
1. Modify the files and [**commit**][ref-commit] changes to complete your solution.
1. [**Push**][ref-push]/sync the changes up to GitHub.
1. [Create a **pull request**][pull-request] on the original repository to turn in the assignment.

### Feedback
After you submit your pull request, the professor will review your code and provide in-line feedback within the pull request. 

### Keeping Your Fork Updated
You'll need to update your fork when we release a new assignment __and__ before you submit anything. You can find instructions for updating or [rebasing your fork __here__][rebase]. Unlike the basic push and pull commands, there are no buttons for these actions in RStudio. You'll need to open the shell by clicking the gear icon in the git panel. Just replace the example upstream repository with the link to this repo. Remember, you only need to do this once.  

> git remote add upstream (repo address)  

Then, every week when you want to update your repository with the new explorations, type this:  

> git fetch upstream  
> git rebase upstream/master  

Note that because you made changes to your files (presumably) when working on the assignment, you may encounter a conflict. There are some options here, but for most students this will work:  
> git rebase upstream/master --autostash  

If you committed your changes (if you were the one that submitted the assignment or you have been backing up your work), then there will be conflicts and rebase will give you an error. Because we do not accept your pull request when you turn in the assignment, you'll have to reset to a version of the repository that corresponds to the upstream branch to rebase properly. You can also '--skip' the conflicts, but this may introduce other issues. Try the following steps to look through your history for the correct commit, reset your branch, and rebase:  
> git log  
> git reset [commit code here - it's a long alphanumeric]  
> git rebase upstream/master  

For more information on how to handle commits, conflicts, and every other type of error that git will throw at you, make sure to refer to the [**git cheat sheet**][git-cheat-sheet] or your favorite google result.  

### Miscellaneous: 
If you are a Mac user using RStudio to push to git via https, you may need to run this:  
>git config --global credential.helper osxkeychain


<!-- Links -->
[download-r]: https://cran.r-project.org/
[download-rstudio]: https://www.rstudio.com/products/rstudio/download3/
[download-git]: https://git-scm.com/downloads
[download-tex]: https://www.latex-project.org/get/
[git-tour]: https://www.youtube.com/watch?v=VUaBfYCmJls
[coatless-presentation]: https://drive.google.com/file/d/0ByNsd8qm6Gepb3RPbllVZ0tpOEU/view
[create-repo]: https://help.github.com/articles/create-a-repo
[add-to-team-action]: https://github.com/education/teachers_pet/#giving-others-access
[forking]: https://guides.github.com/activities/forking/
[ref-clone]: http://gitref.org/creating/#clone
[ref-commit]: http://gitref.org/basic/#commit
[ref-push]: http://gitref.org/remotes/#push
[pull-request]: https://help.github.com/articles/creating-a-pull-request
[markdown-lessons]: http://rmarkdown.rstudio.com/lesson-1.html
[rebase]: https://robots.thoughtbot.com/keeping-a-github-fork-updated
[git-cheat-sheet]: https://services.github.com/kit/downloads/github-git-cheat-sheet.pdf

