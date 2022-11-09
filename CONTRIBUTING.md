# CONTRIBUTING

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

## Setting up the project on a new computer
> INSTRUCTIONS: add link to project box folder below

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
- **You are all set to start working!**

## Workflow

> INSTRUCTIONS: describe project workflow here