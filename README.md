# git_assignment_HeroVired
#git assignment
CalculatorPlus

Baseline scenario:

The application provides basic arithmetic operations, such as addition, subtraction, multiplication, and division. Our task is to implement a new feature that adds support for calculating the square root of a number under a new branch called ‘feature/sqrt’.
"git_assignment_HeroVired" repository is created in Github
cloned repository to local using "Git clone https://github.com/Kavi1312/git_assignment_HeroVired.git
created dev branch using "Git checkout -b dev"
created a python file calc.py with basic arithmetic operations
committed the changes using "git commit -m "committed changes"
Pushed the branch to Github using "git push --set-upstream origin dev"
Merged this to main branch using "git checkout main" and merged to dev 
Created 1st version of release with "Calculatorplus_v1" tag
Added collaberaters 
created feature/sqrt branch using "git checkout -b feature/sqrt" for implementing sqrt functionality
updated the calc.py file with sqrt functionality
committed the changes using "git commit -am "Calcuator with sqrt operations"
Pushed the branch to Github using "git push --set-upstream origin feature/sqrt"
For bug fix in dev branch, "git checkout dev"
Fixed divide functionality and committed & psuhed the changes to remote dev branch
The bug fix is merged to feature/sqrt branch and a pull request with code review is submitted to merge to main branch
After pull request is approved, "feature/sqrt" branch is merged into the ‘dev’ branch.
Dev branch is merged to main branch
Created 2nd version of release with "v2" tag
fixed the bug which is critical
The bug fixation is in the divide function for "Cannot divide by zero", so in case someone enters divisor as 0 we should have a exception rather than breaking the whole scirpt. Due to this bug, we had tostop the sqrt feature and fix this bug 1st.
After fixing the bug, we saw merge conflicts as the changes were in same file.

Resolution
I resolved the bug using Github user interface, by reviewing lines under conflict, view last merged PR with exact changes and remove unwanted branch info/lines.


Git LFS (Large File Storage) integration

Created a new branch "lfs" in local Git "git checkout -b lfs"
Downloaded a large binary file of size > 200 MB
To integrate Git LFS, git lfs track "*.bin" --> extension type
It creates .gitattribute file with detailed of lfs tracked files
add the binary file & .gitattribute file to the repository by following the below steps git add . git commit -m "Adding large binary files to the repository" git push --set-upstream origin lfs
clone the repository in another machine and verified the files are downloaded correctly

Geometry-Calculator

Baseline scenario:

Defined simple class using Python program that calculates the area of a circle and the area of a rectangle. We used Git stash/Git stash apply to manage multiple branch changes simultaneously.
Simultaneously work on 2 branches
"feature/circle-area" to work on the circle area feature.
"feature/rectangle-area" to work on the rectangle area.
Issue Faced
On branch "feature/circle-area", I first created all changes but performed git stash to save all changes on that particular branch only tmeporarily. Moved to create new branch "feature/rectangle-area", and once changes were prepared, I used git stash to save changes on that particular branch only tmeporarily again.
Now once back to branch "feature/circle-area", i used git stash apply to move the branch in time to apply respective changes and performed git add/commit/push. Same goes for branch "feature/rectangle-area" and performed same sequence.
Lastly, on merging 1st branch "feature/circle-area" we could see merge conflicts on 2nd branch "feature/rectangle-area" and resolved the same using Github interface and as per structured code to perform correct are calculations.


Created a new branch named "feature/circle-area" to work on the circle area feature - git checkout -b feature/circle-area
Added a new file "geometry-calculator.py" and added the changes --> git add .
stashed the changes using "git stash" and ensured the working directory is clean using "git status"
Created a new branch named "feature/rectangle-area" to work on the rectangle area --> git checkout -b feature/rectangle-are
Added the rectangle area changes using git add .
stashed the changes using "git stash" and ensured the working directory is clean using "git status"
switched to feature/circle-area using git checkout feature/circle-area
retrieved the stashed changes using "git stash pop"
committed the changes and pushed the changes to remote using --> "git commit -m "message" & git push --set-upstream origin feature/circle-area"
Repeat the same steps from 7 to 9 for feature/rectangle-area
Created pull requests from feature/rectangle-area & feature/circle-area to dev branch and had them reviewed by a peer
Merged the dev branch to main branch
