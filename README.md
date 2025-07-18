# Mini Project - Advanced Linux Commands (Local Setup)

## Project Overview
This project explores advanced Linux commands for managing file permissions, ownership, users, and groups in a WSL Ubuntu environment. It covers `chmod`, `chown`, `sudo`, user management (`adduser`, `usermod`, `passwd`), group management (`groupadd`), and a side hustle task to create a `devops` group, 5 users, their home directories, and set group ownership.

## Setup
- Initiated on Jul 18, 2025, 10:50 AM WAT.
- Used WSL Ubuntu terminal with VS Code, documented in `/mnt/c/Users/User/Documents/Workspace/Shell_AWS_Mini_Project`.

## Execution Steps
1. **File Permissions**:
   - Created `test_script.sh` and `note.txt`, modified permissions with `chmod +x` and `chmod 777`.
   - Tested `chown` (skipped if users/groups not yet created).
   - [Screenshot: `file_permissions_local.png` - Shows `ls -latr` with permissions.]
2. **Superuser Privileges**:
   - Used `sudo` to list `/root` and tested `sudo -i`.
3. **User and Group Management**:
   - Created user `johndoe` with `adduser`, added to `sudo` group, switched with `su`, and updated password.
   - Created `developers` group and added `johndoe`.
4. **Side Hustle Task 3**:
   - Created `devops` group.
   - Created users `mary`, `mohammed`, `ravi`, `tunji`, `sofia`, added to `devops`.
   - Verified home directories (`/home/mary`, etc.) created by `adduser`.
   - Set `devops` group ownership and `g+rw` permissions for each directory.
   - [Screenshot: `group_membership_local.png` - Shows `id mary`.]
   - [Screenshot: `group_ownership_local.png` - Shows `ls -latr /home` with `devops` group.]

## Learning Summary
This project deepened my understanding of Linux file permissions (numeric: 755, 777; symbolic: rwx, r-x) and ownership (`chown`), critical for securing files and directories. I learned to use `sudo` for superuser tasks, manage users (`adduser`, `usermod`, `passwd`) and groups (`groupadd`), and switch users with `su`. The side hustle task reinforced group-based permission management by creating a `devops` group, adding users, and setting group ownership on home directories. WSL Ubuntu posed no significant issues, though `sudo` access was crucial. This experience solidified my system administration skills for DevOps workflows.

## Tools Used
- **WSL Ubuntu Terminal**: For executing Linux commands.
- **VS Code**: For editing `README.md`.
- **Git Bash**: For version control and GitHub push.

## Project Deliverables
- **Documentation**: This `README.md` with steps and learning summary.
- **Screenshots**:
  - `file_permissions_local.png`
  - `group_membership_local.png`
  - `group_ownership_local.png`
- **Script Link**: [GitHub Repository](https://github.com/westgrin/Shell_AWS_Mini_Project)

## Conclusion
This project successfully explored advanced Linux commands for permissions, ownership, and user/group management, completed the side hustle task, and documented the process locally. It enhanced my ability to manage Linux systems securely and efficiently.