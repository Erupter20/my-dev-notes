### **Version Control System (VCS)**

- **Why VCS?** To track changes in your codebase over time. Essential for collaboration and managing complex projects.
    
- **Core Concepts:**
    
    - **Branching:** Create an isolated copy ("branch") of your code to work on a new feature without affecting the main codebase.
        
    - **Commits:** Save a snapshot of your changes with a descriptive message.
        
    - **Pull Request (PR):** A request to merge your changes from your branch into the main branch. Allows for code review.
        
    - **Merge Conflicts:** Occur when changes on your branch conflict with changes on the main branch. You must resolve these manually.
        
    - **Rollback:** Revert the codebase to a previous version if a bug is introduced.
        
- **Git vs. GitHub:**
    
    - **Git:** A command-line tool (CLI) for version control installed on your local machine.
        
    - **GitHub:** A web-based platform (GUI) that hosts your Git repositories, enabling collaboration, issue tracking, and more.
        

### **Git Setup & Commands**

1. `git config --global user.name "Your Name"`: Sets your name for all commits.
    
2. `git config --global user.email "your.email@example.com"`: Sets your email.
    
3. `git init`: Initializes a new Git repository in your current folder.
    
4. `git add .`: Stages all changed files, preparing them for a commit.
    
5. `git commit -m "Your descriptive message"`: Saves your staged changes to the repository's history.
    
6. `git branch -M main`: Renames the default branch from `master` to `main` (modern standard).
    
7. `git remote add origin <URL>`: Connects your local repository to a remote one on GitHub (the `<URL>`).
    
8. `git push -u origin main`: Pushes your commits to the `main` branch on the remote repository (`origin`). The `-u` flag sets it as the default for future pushes.
    
9. `git push -u origin main --force`: **Use with extreme caution.** Overwrites the remote history with your local history. Can cause problems for collaborators.