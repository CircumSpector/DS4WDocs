# Backing up, restoring or deleting user data and settings

## User data's files and folders

The complete list of user data related files and folders is the following: 

- Actions.xml
- Auto Profiles.xml
- ControllerConfigs.xml
- LinkedProfiles.xml
- OutputSlots.xml
- Profiles.xml
- Profiles folder

### Backup

It's necessary to verify if there are user related data in two different folders: inside the main DS4Windows folder and in the user's Profile folder. To do so:

1. Click on the `Profile Folder` option under DS4Windows' `Settings` tab and confirm if the user related data is there
1. Also check if the user data is on DS4Windows' main folder, even if you found data previously on the Profile folder
1. If both locations contains user data related files then the actual location used by DS4Windows load User Data is the one that cointains the `Profiles.xml` file
    - If the user plans to backup the entirity of DS4Windows and the User Data location is on the DS4Windows folder itself then they can just backup the whole folder
1. After finding the actual location User Data is loaded from, backup the related files and folders presented on the main section's list

### Restore

- Copy the user data back to the profile folder or to the main DS4Windows folder accordingly to your use case, then restart DS4Windows if it's open
- If both locations contain user data DS4Windows will prompt the user to choose which place to load from. Most of the user data on the unused location will then be deleted

### Delete

Follow the same steps as on the Backup section, but delete the found User Data.






