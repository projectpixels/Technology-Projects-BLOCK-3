# Understanding File Permissions

## Task 1 --- Create a File

Run:

    touch secret.txt
    ls -l secret.txt

### Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/bc477855-a5ca-4034-ba8f-5cb48b5ccfbd" />


### Questions

1.  Who owns the file?
   ans= The user who created it, shown in the 3rd column of ls-l
3.  What are the default permissions?
    ans= Usually -rw-r--r-- (644)
### Reflection

Why is file ownership important in Linux systems?
ans= File ownership decides who can read, change or run a file. It enforces access control, so users can't access each other's file and a compromised account can only reach what that user owns.
------------------------------------------------------------------------

## Task 2 --- Restrict File Permissions

Run:

    chmod 600 secret.txt
    ls -l secret.txt

### Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/720258f4-7dee-4417-9af2-a544e495f389" />


### Questions

1.  Who can read the file now?
   ans= bitmasters
2.  Who cannot access it?
   ans= the group and all other users have no read, write or execute access.


------------------------------------------------------------------------

## Task 3 --- Open Permissions (Security Risk)

Run:

    chmod 777 secret.txt
    ls -l secret.txt

### Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/153bb83f-3fe3-41a7-83b6-2ad4cb53b9de" />


### Questions

1.  Who can access the file now?
   ans= Everyone
3.  Why might this configuration be dangerous?
ans= Any user or compromised process on the system can read the secret data, modify or delete the file, or replace it with malicious content.
