**Set Up a Repository**:
   - Create a new repository on GitHub or use an existing one.
   - Clone the repository to your local machine:
     ```bash
     git clone https://github.com/username/repo.git
     cd repo
     ```

2. **Create and Switch to `feature-branch-1`**:
   - Create a new branch and switch to it:
     ```bash
     git checkout -b feature-branch-1
     ```

3. **Make Changes in `feature-branch-1`**:
   - Edit a file (e.g., `file.txt`):
     ```bash
     echo "Changes from feature-branch-1" >> file.txt
     ```
   - Commit the changes:
     ```bash
     git add file.txt
     git commit -m "Changes from feature-branch-1"
     ```
   - Push the branch to GitHub:
     ```bash
     git push origin feature-branch-1
     ```

4. **Create and Switch to `feature-branch-2`**:
   - Switch back to the main branch and create another branch:
     ```bash
     git checkout main
     git pull origin main
     git checkout -b feature-branch-2
     ```

5. **Make Conflicting Changes in `feature-branch-2`**:
   - Edit the same file (`file.txt`) differently:
     ```bash
     echo "Changes from feature-branch-2" >> file.txt
     ```
   - Commit the changes:
     ```bash
     git add file.txt
     git commit -m "Changes from feature-branch-2"
     ```
   - Push the branch to GitHub:
     ```bash
     git push origin feature-branch-2
     ```

6. **Create a Pull Request for `feature-branch-1`**:
   - Go to GitHub and create a pull request from `feature-branch-1` into `main`.

7. **Create a Pull Request for `feature-branch-2`**:
   - Go to GitHub and create a pull request from `feature-branch-2` into `main`.

8. **Attempt to Merge Both Pull Requests**:
   - When you attempt to merge `feature-branch-1`, it will succeed if there are no conflicts.
   - Next, try to merge `feature-branch-2`. GitHub will detect a conflict because both branches made changes to the same line in `file.txt`.

### **Resolving the Conflict**

**1. Resolve Conflict Locally**:
   - **Fetch and Check Out the Branch with the Conflict**:
     ```bash
     git checkout feature-branch-2
     git pull origin feature-branch-2
     ```

   - **Merge the Main Branch**:
     ```bash
     git fetch origin
     git merge origin/main
     ```
     This will result in a conflict since `file.txt` has changes from both branches.

   - **Resolve the Conflict**:
     - Open the conflicting file (`file.txt`). Git marks the conflict areas with conflict markers:
       ```
       <<<<<<< HEAD
       Changes from feature-branch-2
       =======
       Changes from feature-branch-1
       >>>>>>> main
       ```
     - Edit the file to resolve the conflict. For example:
       ```text
       Changes from feature-branch-1
       Changes from feature-branch-2
       ```
     - Save the file and remove the conflict markers.

   - **Add and Commit the Resolved File**:
     ```bash
     git add file.txt
     git commit -m "Resolved conflict between feature-branch-1 and feature-branch-2"
     ```

   - **Push the Resolved Changes**:
     ```bash
     git push origin feature-branch-2
     ```

**2. Merge the Pull Request on GitHub**:
   - Return to GitHub and merge the pull request for `feature-branch-2` into `main`. The conflict should be resolved now.

### **Summary**

- **Create a Conflict**: Make conflicting changes in different branches and try to merge them.
- **Resolve a Conflict**: Fetch the branches, attempt to merge, edit the conflicting files, and commit the resolved changes.
