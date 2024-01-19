# Linux-Project
File permissions in Linux

## Project Description

The team at my organization needs to update the file permissions for certain files and directories within the /projects directory. Examined and managed the permissions on the files in the /home/researcher2/projects directory for the researcher2 user. I checked the permissions for all files in the directory, including hidden files and made sure that permissions align with the authorization that should be given. 
![image](https://github.com/ljmbriones/levibriones/assets/151262749/4789c3f2-76cd-4ac7-99a3-0606f392df2e)

## Describe the permissions string
In the /home/researcher2/projects directory, there are five files with the following names and permissions: 
- project_k.txt
  - User = read, write, 
  - Group = read, write
  - Other = read, write
- project_m.txt
  - User = read, write
  - Group = read
  - Other = none
-  project_r.txt
  - User= read, write
  - Group = read, write
  - Other = read
- project_t.txt
  - User = read, write
  - Group = read, write
  - Other = read
- .project_x.txt
  - User = read, write
  - Group = write
  - Other = none
 
## Change file permissions
None of these files should have Write permissions for Other users. Checked that file project_k.txt has Write permission for Other users. Changed permission by using chmod command. Listed them using ls -la command to confirm changes

![image](https://github.com/ljmbriones/levibriones/assets/151262749/71786fa8-62e1-4ebc-96e3-2ae3b2a48864)
- Project_m.txt also is a restricted file and should not be readable or writable by group or other. Changed permissions:

![image](https://github.com/ljmbriones/levibriones/assets/151262749/a678dfb7-41fa-4353-a309-210cbb1147bd)

## Change file permissions on a hidden file
The file .project_x.txt is a hidden file that has been archived and should not be written to by anyone. Used chmod command to remove user and group Write permissions
![image](https://github.com/ljmbriones/levibriones/assets/151262749/afebd282-a85b-4930-9f07-60420017f063)

Changed permission for User and Group to have Read permissions:
![image](https://github.com/ljmbriones/levibriones/assets/151262749/326cfb4e-6946-433d-b536-65b40014af41)

## Change directory permissions
Removed the execute permission for the group from drafts directory:
![image](https://github.com/ljmbriones/levibriones/assets/151262749/bb6161ea-3d2c-4e53-8c4c-0fa4b89e5d68)

# Summary
Experienced in using basic Linux Bash shell commands to do the following:
Examined file and directory permissions, changed permissions on files, and changed permissions on directories
