# GettingStarted
Getting Started with Git / GitHub
Steps:
1. Download/install Git and set up your global username and employee email(keep in mind that other people will be viewing your edits by your user name).
2. Create a free GitHub account using your employee email.
3. Download/install Visual Studio Code

    [Follow these simple rules and you’ll become a Git and GitHub master - Aerial Camus](https://www.freecodecamp.org/news/follow-these-simple-rules-and-youll-become-a-git-and-github-master-e1045057468f/)

    1. Create a GitHub repository for every new project
    2. Create a new branch for every new feature
       1. Clone a branch from the "company" repo into your local repo
       2. Commit edits/additions in your local repo 
    3. Use Pull Requests to merge code to Master

## git
website: https://git-scm.com/downloads

Getting Started Video: https://git-scm.com/video/get-going

Cheatsheet: https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf

Notes:
**Set up global git environment**
```cmd
git config --global user.name "Your User Name"
git config --global user.email "UserName@gmail.com"
```
**Verify global environment**
```cmd
git config --list
```
**gitignore**
Projects which contain sensitive information and/or local builds and compiled code must include a gitignore file to explicitly prevent specified folders, files or file types from being both tracked in git and added to the GitHub repository.  All builds and information containing database connection strings secrets and passwords should ONLY exist in your local build and must be excluded via gitignore.  A readme file should instruct the user of the necessary steps to "wire" up the project.  


## GitHub
website: https://github.com/

Getting Started Videos: 
https://www.youtube.com/watch?v=0fKg7e37bQE
https://www.youtube.com/watch?v=x0EYpi38Yp4

https://guides.github.com/activities/hello-world/
Cheatsheet: 

Notes:

### Markdown
website: https://www.markdownguide.org/getting-started

Getting Started Video: 

Cheatsheet: https://www.markdownguide.org/cheat-sheet

Notes:

### GitHub Desktop
website: https://desktop.github.com/

Getting Started Video: https://www.youtube.com/watch?v=S7f8qJscmRE

Cheatsheet: 

Notes:

Excerpt from https://github.com/desktop/desktop/edit/development/docs/process/what-is-desktop.md
#### What is GitHub Desktop and who is it for?

##### Purpose
As we triage issues, evaluate pull requests, and discuss new features, the GitHub Desktop team is 
making decisions based on our vision for the GitHub Desktop product. The purpose of this document 
is to transparently share our collective view of what GitHub Desktop is and who we’re optimizing 
for when making decisions. Our goal is to be able to point back to this document to ensure there are 
fewer surprises and that we’re consistent in our product decisions. This will likely evolve 
over time as we continue to learn more about our users and the problem space.

##### 1. GitHub Desktop reduces frustration and makes Git and GitHub workflows* more approachable.

Our goal with GitHub Desktop is to remove frustration, awkward interactions, and “oh no” moments 
for as many people as possible. We aim to make common workflows* (defined at the end of this document) 
so simple that beginner and experienced developers alike are productive in working with Git and GitHub. 
Git can be intimidating, and we want GitHub Desktop to make interactions with Git easier and more 
approachable. GitHub Desktop is not a replacement for the functionality of Git, but a tool to enable 
you and your team to be more productive.

###### 2. GitHub Desktop extends GitHub to your local environment.

GitHub Desktop is built and maintained by a team at GitHub and a group of amazing community contributors 
as an open source application. It is intended primarily to extend the features of GitHub, not to be an 
agnostic Git client or replicate the feature set of github.com. While we support very basic functionality 
that will allow the app to function with other hosting providers, we prioritize work that allows the 
end-to-end GitHub and GitHub Enterprise experience to shine and takes advantage of the fact that we can 
closely integrate with GitHub features.

###### 3. GitHub Desktop prioritizes workflows for beginners and collaborative teams.

We want to create an inclusive and approachable way for developers to turn ideas into reality, and we see 
GitHub Desktop as critical in reducing the intimidation of working with Git on the command line. Users of 
all experience levels will continue to benefit from GitHub Desktop’s features but when we have to choose 
between workflows for advanced Git users and workflows for beginner Git users, we prioritize beginners. 
Additionally, we think it’s foundational to support solo development, but our unique value comes from combining 
the power of GitHub with the convenience of working locally so that you can collaborate with your team easily. 
This also means GitHub Desktop will likely not support workflows that are unique to your team, against 
documented best practice, or different from the vast majority of developers.

###### 4. GitHub Desktop has a variety of people using it, but our core users are software developers.

GitHub has millions of possible use cases and we believe that nearly every industry should be using Git. 
We support its versatility, but when we have to make choices about whose workflows to prioritize, 
we prioritize those for software developers.

###### 5. GitHub Desktop is a tool that enables you to learn while you get things done

GitHub Desktop should be a helpful tool for beginner developers, but it is not explicitly a teaching tool. 
It is fundamentally to help you get your work done faster and more effectively, in a way that is consistent 
with and encourages best practices.

&nbsp;&nbsp;&nbsp;&nbsp;

*We define a workflow as a path that users take toward achieving a particular goal. An example is a “merge” 
workflow, where the goal is to bring work together that was done in different places.

### Visual Studio Code
website: https://code.visualstudio.com/Download

Getting Started Video: https://code.visualstudio.com/docs/introvideos/basics

Cheatsheet: https://github.com/microsoft/vscode-tips-and-tricks

**Notes:**

**Steps to clone a GitHub Repository:**

1. Create a directory on the local file system.
2. Create a repo on Github.
3. Select Clone "Clone or download" on Github, copy the link
4. In **Visual Studio Code**, select _File_ -> _Add Folder to Workspace_ -> Select the newly created directory
5. Select Terminal Window
    In the window, type:
    ```
    git config global user.name [github userID]
    git clone [URL from github link copied earlier]
    ```
**Adding an existing project to GitHub using the command line:**
  gsantopaolo    October 12, 2018 0 2,245   Less than a minute
1. Create a new repository on GitHub. 
    * Add a gitignore file(see sample gitignore templates).
    * Add a readme file if none exists in your local project.
    * Add a licence if you want.
2. Open Git Bash
3. Change the current working directory to your local project.
4. Initialize the local directory as a Git repository.
```
git init
```
5. Add the files in your new local repository. This stages them for the first commit.
```
git add .
```
6. Commit the files that you’ve staged in your local repository.
```
git commit -m "initial commit"
```
7. Create a new repository in the morris-county-gis group
        *Click the new repository button in the top-right. Initialize the repository with a README file.
        *Click the “Create repository” button.
        *Note: there may be a button that you can press to copy the URL needed in the next step.
        
8. Copy the https url of your newly created repo

    * In the Command prompt, add the URL for the remote repository where your local repository will be pushed.
    ```
    git remote add origin [remote repository URL]  https://github.com/[user]/[repoName]
    ```
git remote -v

9. Push the changes in your local repository to GitHub.

git push -f origin master

        
