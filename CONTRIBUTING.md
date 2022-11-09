# CONTRIBUTING

- [Setting up the project on a new computer](https://github.com/DevInnovationLab/dil-template-repo/edit/contributing/CONTRIBUTING.md#setting-up-the-project-on-a-new-computer)
- [Workflow](https://github.com/DevInnovationLab/dil-template-repo/edit/contributing/CONTRIBUTING.md#workflow)
- [Folder structure](https://github.com/DevInnovationLab/dil-template-repo/edit/contributing/CONTRIBUTING.md#folder-structure)
- [Naming conventions](https://github.com/DevInnovationLab/dil-template-repo/edit/contributing/CONTRIBUTING.md#naming-conventions)

## Setting up the project on a new computer

> INSTRUCTIONS: add link to project box folder on the next line
- [ ] If you don't have the Box client installed, install it and sync the [project's Box folder](link to project box folder)
- [ ] If you don't have a local git client installed, install one (e.g. [GitHub Desktop](https://desktop.github.com/))
- [ ] Clone this repository: click on the green *Code* button, then *Open with GitHub Desktop* 
- [ ] Using the GitHub client, check out the `develop` branch
- [ ] Navigate to the local copy of the repository 
> INSTRUCTIONS: edit the lines below to reflect the preferred [file path](https://dimewiki.worldbank.org/File_path) handling solution for the project by keeping only one of the next two items
- [ ] Add your computer's username and file paths to the [main script](link to master script lines to be edited) and commit your changes
- [ ] Create a directory junction or symlink to the Box data folder on the root directory for the repo:
```
# Mac
ln -s /your/git/repo/clone/data/ /data/folder/on/your/box/folder/

# PC
mklink /J /your/git/repo/clone/data/ /data/folder/on/your/box/folder/
```
- [ ] Change the options in the main script in order to re-run the whole code for the paper, from importing the raw data to recreating any intermediate and final datasets, to exporting any results
- [ ] Delete any code outputs, including all derived data sets, all tables and all figures exported by the code
- [ ] Run the main script
- [ ] Check that:
  - [ ] The code ran, that is, there was no error message
  - [ ] All code outputs were recreated. If any file was not recreated, it will show as red on the git client.
  - [ ] There are no changes in the outputs or you can tell where they are coming from. If there are changes, commit the changes and explain in the commit message where the changes are coming from

**You are all set!**

## Workflow

> INSTRUCTIONS: describe the project's implementation of [gitflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) here. Below is an example

The `main` branch in this repository is protected. All changes to the main branch should come from *pull requests* (PR) from the `develop` branch. **The `develop` branch should be merged to master after (1) completing the data processing for a new data source; (2) developing a new piece of analysis; completing a round of code review.** Once one of these tasks is complete:
 - [ ] Using the `develop` branch, run the entire project code from the main script.
 - [ ] Still on the `develop` branch, update the README file.
 - [ ] Push your changes.
 - [ ] Open a *pull request* (PR) to the develop branch. Link to all the *issues* addressed in this PR on the PR message.
 - [ ] Assign a reviewer and let the reviewer know on Slack that they have been assigned a new PR. *List here the handles of team members that can review pull requests to `main`.*


**Day-to-day code should be developed on feature branches and merges to `develop` around twice a month.** Break large tasks into smaller tasks, taking one to two weeks of work, and work on them one at a time, with a different feature breanch for each. Once the task in a feature branch is complete:
 - [ ] Using the feature branch, run the entire project code from the main script. If there are computationally intensive steps that were not edited, you may skip them. Do this at least twice, committing changes between runs to ensure the code is stable.
 - [ ] Still on the feature branch, update the README file.
 - [ ] Push your changes.
 - [ ] Open a *pull request* (PR) to the develop branch. Link to all the *issues* addressed in this PR on the PR message.
 - [ ] Assign a reviewer and let the reviewer know on Slack that they have been assigned a new PR. *List here who are the team members that can review pull requests to develop -- it can be anyone in the team who is knowledgeable of the coding language used.*


 
## Folder structure

> INSTRUCTIONS: Describe folder structure here or link to the template adopted

## Naming conventions

> INSTRUCTIONS: Describe naming conventions for each type of name

### Folders

### Files

- Code
- Data
- Documentation

### Variables

### Functions
