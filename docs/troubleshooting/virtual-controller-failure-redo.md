# DS4Windows not creating virtual controllers

!!! important "Under construction ⚒️"

## Starting point

This page takes account that DS4Windows successfully detects your controller and starts as normal without error messages in the `Log` tab. 

TO DO: Also, that you are not facing physical issues with your controller.

If DS4Windows is failing to start or is starting but creating error messages in the log, firstly refer to the [_DS4Windows does not open, crashes or cannot start_ page]().

## Verifying if DS4Windows is successfully creating virtual controllers

DS4Windows cannot magically change your real controller to one for another type, so what it actually does is create a virtual Xbox or DS4 controller that is then associated to your real one. If the virtual controller creation fails then one of DS4Windows main features is not working.

To confirm everything is working:

!!! important "Follow this carefully and step-by-step!"

- Let DS4Windows running but __stop__ it by pressing the dedicated `Stop` button
- Open Windows' Game Controller list
- Make a mental note on what controllers are on the list
- Back on DS4Windows, Check the state of the `Hide DS4 controllers` option in the `Settings` tab. Disable it for now if it's enabled
- Start DS4Windows again
- On the `Log` tab more recent messages, check if the following messages exist:
``` 
Plugging in virtual (X360/DS4) Controller
Associate (X360/DS4) Controller in slot #X for input (your real controller type) controller #X
``` 
- Confirm on Windows' Game Controllers list if the new virtual controller has now been detected

### The "Associate (X360/DS4) Controller (...)" message appears on the log but the virtual controller does not appear on the Game Controllers list

Maybe the user has accidentally hidden the virtual controller with HidHide? In most cases, HidHide should be used to hide only real devices, though virtual devices will also appear on the list and can be hidden as well.

To test if this is the case, open HideHide Configuration Client and temporarily disable it by unticking the `Enable device hiding` checkbox and check on the Game Controllers list again. If the virtual controller was hidden then it should appear now. Keep in mind that if your real controller was hidden then it will also re-appear on the list.

If you found out this was your case then re-tick the `Enable device hiding` checkbox and re-do your HidHide' hidden devices list so only real, physical controllers are selected.

For other situations...?

!!! note "To Do"

### The "Associate (X360/DS4) Controller (...)" does NOT message appears on the log

It's possible that the user has disabled virtual controller creating/association in the currently active profile. To verify:

- Go into DS4Windows' `Controllers` tab
- Click on the `Edit` button next to the selected profile
- Check on the `Profile editor -> Other` tab if the `Disable virtual controller` checkbox is ticked. Untick it if applicable
- Save the profile changes and stop/start DS4Windows
- Confirm on Windows' Game Controllers list if the new virtual controller has now been detected