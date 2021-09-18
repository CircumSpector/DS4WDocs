# DS4Windows not creating virtual controllers

!!! important "Under construction ⚒️"

## IMPORTANT, START HERE!

- This page takes account that DS4Windows successfully detects your controller and starts as normal without error messages in the `Log` tab
    - If DS4Windows is failing to start or is starting but creating error messages in the log, firstly refer to the [_DS4Windows does not open, crashes or cannot start_ page]().
- It's also considered that your real controller can be detected by DS4Windows and works as normal on the [Gamepad Tester Website](https://gamepad-tester.com/)
    - To make a full controller check to verify that the controller is not exhibiting a physical issue, refer to [this page](../../under-construction)

!!! info "To Do"
    section under construction, topics to include:
    - Make sure the `Hide DS4 option` is not being used when troubleshooting this since the user might mistake their real controller with a virtual one when stopping DS4Windows and the device is un-hidden
    - Other remarks?

## Verifying if DS4Windows is successfully creating virtual controllers

DS4Windows cannot magically change your real controller to one for another type, so what it actually does is create a virtual Xbox or DS4 controller that is then associated to your real one. If the virtual controller creation fails then one of DS4Windows main features is not working.

To confirm everything is working:

!!! info "To Do"
    Section under construction

### The "Associate (X360/DS4) Controller (...)" message appears on the log but the virtual controller does not appear on the Game Controllers list

!!! note "To Do"
    Section under construction. Topics to include:
    - ViGEm spawned the device but it's in a error state. Verify on Device Manager
    - Check ViGEm log
    - Virtual controller has been hidden by HidHide/HidGuardian?
    - HidHide HidGuardian issue that can happen when the user has both installed at the same time
    - Other?

### The "Associate (X360/DS4) Controller (...)" does NOT message appears on the log

It's possible that the user has disabled virtual controller creating/association in the currently active profile. To verify:

- Go into DS4Windows' `Controllers` tab
- Click on the `Edit` button next to the selected profile
- Check on the `Profile editor -> Other` tab if the `Disable virtual controller` checkbox is ticked. Untick it if applicable
- Save the profile changes and stop/start DS4Windows
- Confirm on Windows' Game Controllers list if the new virtual controller has now been detected