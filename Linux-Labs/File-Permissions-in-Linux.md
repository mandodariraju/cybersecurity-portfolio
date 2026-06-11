# File Permissions in Linux

## Project Description

The research team at my organization needed to update file and directory permissions within the projects directory. The existing permissions did not reflect the appropriate authorization levels. To improve security, I reviewed and modified permissions using Linux commands.

---

## Check File and Directory Details

I used the following command to review files, directories, and their permissions:

```bash
ls -la
```

This command displayed all files, including hidden files, and showed detailed permission settings for each item.

---

## Understanding Permission Strings

Linux permissions are represented by a 10-character string.

Example:

```text
-rw-rw-r--
```

- First character (`-`) indicates a regular file.
- Characters 2-4 represent user permissions.
- Characters 5-7 represent group permissions.
- Characters 8-10 represent permissions for others.

Permission symbols:

- `r` = Read
- `w` = Write
- `x` = Execute
- `-` = Permission not granted

---

## Removing Write Access for Others

The organization required that users categorized as "others" should not have write access to project files.

Command used:

```bash
chmod o-w project_k.txt
```

This removed write permissions for other users while preserving existing permissions for the owner and group.

---

## Updating Permissions on a Hidden File

The file `.project_x.txt` was archived and needed stricter permissions.

Requirements:

- User: Read only
- Group: Read only
- Others: No access

Commands used:

```bash
chmod u-w .project_x.txt
chmod g-w .project_x.txt
chmod g+r .project_x.txt
```

These changes removed unnecessary write permissions and ensured appropriate access levels.

---

## Restricting Directory Access

The organization required that only the `researcher2` user should have access to the `drafts` directory.

Command used:

```bash
chmod g-x drafts
```

This removed execute permissions from the group while maintaining access for the authorized user.

---

## Skills Demonstrated

- Linux File Permission Management
- Access Control
- Principle of Least Privilege
- Security Hardening
- Linux Command Line Operations
- chmod Command Usage
- Directory Permission Management

---

## Commands Used

```bash
ls -la
chmod o-w project_k.txt
chmod u-w .project_x.txt
chmod g-w .project_x.txt
chmod g+r .project_x.txt
chmod g-x drafts
```

---

## Summary

This project involved reviewing and updating Linux file and directory permissions to align with organizational security requirements. By applying the principle of least privilege and using Linux permission management tools, I improved access control and strengthened system security.
