## User and Group Management Project
### Step 1: Access the Linux System
- For this project, make use of a Vagrant Linux box and access it using <code>vagrant ssh</code>

![screenshot-1](accesslinux.JPG)

### Step 2: Open a Terminal
- If you're not already in a terminal session, open a terminal window. You'll use this terminal to execute user and group management commands.

![screnshot-2](accesslinux.JPG)

### Step 3: Create a New User
- Create a new user using the useradd command. Replace newuser with the desired username.

    > sudo useradd newuser

![screenshot-3](useraddnewuser.JPG)

### Step 4: Set a Password for the New User
- Set a password for the new user using the passwd command:

    > sudo passwd newuser

![screenshot-4](newuserpasswd.JPG)

### Step 5: Create a New Group
- Create a new group using the groupadd command. Replace newgroup with the desired group name.

    > sudo groupadd newgroup

![screenshot-5](useraddnewgroup.JPG)

### Step 6: Add User to a Group
- Add the newly created user to the group using the usermod command. Replace newuser with the username and newgroup with the group name.

    > sudo usermod -aG newgroup newuser

![screenshot-6](newusertonewgroup.JPG)

### Step 7: Verify User and Group Creation
- Check if the new user and group have been created successfully:

    >   id newuser
        
        getent group newgroup

    ![screenshot-7](userandgroupverify.JPG)

### Step 8: Modify User and Group Information
- You can modify user and group information using the usermod and groupmod commands. For example, to change the user's home directory:


    >   sudo usermod -d /new/home/directory newuser

![screenshot-8](modifyuserandgroupinfo.JPG)

### Step 9: Delete a User
- To delete a user, use the userdel command. Be careful, as this will remove the user account.

    >   sudo userdel -r newuser

![screenshot-9](userdelnewuser.JPG)

### Step 10: Delete a Group
- To delete a group, use the groupdel command. Be cautious, as this will remove the group.

    >   sudo groupdel newgroup

![screenshot-10](userdelnewuser.JPG)

