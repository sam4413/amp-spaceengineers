# Regular Windows AMP for Space Engineers Torch
## Please note, Torch on AMP does not officially support this out of box, and this guide was made by a member of the Space Engineers community. For a seamless out of box experience, please use the Windows Server versions.

1. Create new local user that AMP runs on. `net user AMP amppassword /add`<br>
You need to do this, because AMP can’t run on an admin account.

2. Go to where your AMPDatastore folder is, right click and select “Properties”

![image](https://github.com/user-attachments/assets/5f0552e3-c0d2-4d6c-946f-b1b093bad2dd)

3.Click on “Security”, then “Advanced at the bottom”

![image](https://github.com/user-attachments/assets/dad435cb-e6d9-4b70-af8f-149cf559e244)

4. Click “Change”, then type in your new username (AMP in this example)

![image](https://github.com/user-attachments/assets/cb315015-e42e-41c6-9121-1f0d478ffad6)

5. After selecting “OK”, click the Replace Owner and Replace all child object checkboxes.

![image](https://github.com/user-attachments/assets/e30e4e14-0533-4e5a-a06c-df1362d6f242)

Let windows change permissions, this can take several minutes depending on your specs and the size of amp’s datastore.

6. Now, Press Windows Key + R, then services.msc. Find “AMP-ADS01”, right click and click “Properties”. Change “Startup Type” to Manual, then stop the service.

![image](https://github.com/user-attachments/assets/9f5a8fcf-1ff0-4b16-8e75-74ff2b6f6e96)

7. Go to the Task Scheduler, on the right select “Create Task”, not Basic Task. Name it anything you want. In “Security Options” towards the bottom, Click “Change User” and select your newly created user.

![image](https://github.com/user-attachments/assets/41fed4ac-21cd-4836-8d0f-0303cc2e6a7e)

8. Go to “Triggers” at the top, and create a new trigger that runs at log on, click on “Specific User” and change the user to match your new user.

![image](https://github.com/user-attachments/assets/1c5f1242-f2b6-4cc1-a564-8355c0d5829f)

9. Go to “Actions” and create a new action. The Action type needs to be “Start a program”, and the program location needs to be AMP’s exe. Usually it will be in C:\AMPDatastore\Instances\ADS01\AMP.exe (Or in your largest drive depending on how you installed AMP).

![image](https://github.com/user-attachments/assets/784bc088-8736-4b1f-8216-3e56cdf7e6e1)

10. Restart your computer and log in as your new user, you will see AMP start in the command line, then you can load your Torch instances without issues.
