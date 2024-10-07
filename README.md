# Git Summary Notes (202434681 HongSeungWoo)

## 1. Version Control and Collaboration
- Version control systems are essential for software development and document management.
- **Basic Solution**: Making multiple copies of files.
- Systematic management is necessary.

## 2. Changes vs Snapshots
- **Changes**: Storing differences from the base version.
- **Snapshots**: Storing the full state of the project at specific points in time.

## 3. Types of Version Control Systems
### Local Version Control
- **Description**: All versions stored on the local machine.
- **Advantages**:
  - Fast and easy to use.
  - No network required.
- **Disadvantages**:
  - Hard to share changes with others.
  - Risk of data loss if the local machine fails.

### Centralized Version Control
- **Description**: All versions stored on a central server.
- **Advantages**:
  - Easy to manage user permissions.
  - Simplified collaboration through a central server.
- **Disadvantages**:
  - Single point of failure (if the server goes down, no one can access the repository).
  - Requires a network connection for most operations.

### Distributed Version Control
- **Description**: Every user has the full version history on their machine (e.g., Git).
- **Advantages**:
  - Users can work offline and have complete history.
  - Better collaboration and branching capabilities.
- **Disadvantages**:
  - Can be complex to learn for new users.
  - May lead to larger storage requirements on local machines.

## 4. Three States in Git
- **Modified**: Files that have been changed but not yet added to version control.
- **Staged**: Files marked to be committed.
- **Committed**: Files that are safely stored in the Git repository.

## 5. Git Configuration (First-time Setup)
- Configuration is stored at three levels:
  - **System Level**: Applies to all users on the system.
  - **Global Level**: Applies to a specific user.
  - **Local Level**: Specific to a single repository.
- Set your username and email:
  - `git config --global user.name "Your Name"`
  - `git config --global user.email "your.email@example.com"`

## 6. Git Workflow Example
1. **Initialize Repository**: use `git init`
2. **Check Repository Status**: Check the current status of the repository. usr `git status`
3. **Add Files to Staging**: 
   - Add specific files. use `git add [file_name]`
   - Add all files. use `git add .`
4. **Unstage Files**: Unstage files that have been added to staging. use `git rm --cached [file_name]`
5. **Ignore Files**: Use a `.gitignore` file to specify files to be ignored.
6. **Commit Changes**: Commit the changes made. use `git commit -m “commit message”`
