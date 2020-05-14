# GitHub Tips

* Whenever you create a new repository **seed** it with a *readme.md* file and *gitignore* file in the root folder.

* Your scripts and web projects should reside in a sub-folder so that project build and config files don't clutter the root directory of the repository.

* Once you create your blank **seed** repository, clone it to your local workenvironment, then copy or create your project in the sub-folder that you designated, above.

* More than one code project can live in a repository, but the projects should be closely related or coupled....otherwise put them in their own repositories.

* When you have your basic workfiles laid out in your local repo - __*Push*__ your local updates up to GitHub (master).

* At this point, you're ready to begin a more *task-driven* development process by creating a **branch** for each feature or workitem that you're trying to implement and working within your branch.

---

## GitHub Branches
With a basic project created in a single **master** branch of your repository, you're further __development__ *(adding new functionality)* or __maintenance__ *(updating application framework or code libraries)* should be performed in new branches that are appropriately named for the tasks at hand.  As an example, a branch named *"modIVreport-workitem"* could represent a branch where a new modIV report is being designed and added to a website.  

At this point, you'll be in a maintenance cycle, not only with your code, but also with your repository and its branches.   As you perfect code in a working branch, you'll need to merger it into the master branch.   At time's, especially when there are multiple active branches open, you'll want to merge updates that were added to the master branch into your working branch.  These two tasks are very different, in that NO incomplete or breaking code should ever be pushed into a working master branch, and the administrator of the repository should ALWAYS be on-board with a merge into the master.

---

### Merge Branches into the Master Branch in GitHub using Pull-Requests


__*NOTE*__: Whereas every repository has a primary administrator, merges into the master branch MUST always be approved/coordinated by that administrator. 

Example: [https://developers.sap.com/tutorials/webide-github-merge-pull-request.html]
1. **Step 1:** Open __branch__ on __GitHub__. Open the Organization repository on GitHub and switch to the __branch__ that you want to merge into __master__.
2. **Step 2:** Create pull request. Click __New Pull Request__ to create a pull request. ...  
  * Enter brief details about the pull request and click Create pull request. You can scroll down and see a diff of the files that were changed as well as the commits.  
  * If there are no conflicts, you'll be able to complete the pull request, however if conflicts exist between the master and the branch - then each conflict will need to be resolved before completing the pull request.  
  * If all conflicts have been resolved, Click __Create pull request__  
3. **Step 3:** __Merge__ pull request. ...  
  *    If you're satisfied with the changes that will be implemented to the master, click __Merge pull request__  
  *    Click __Confirm merge__  

At this point your __branch__ content should be in the __master_, and the merge is completed.   If you're done with the task - delete the branch, otherwise continue to develop in the branch.


### Merge the Master Branch into your Workitem Branch in GitHub using Pull-Requests