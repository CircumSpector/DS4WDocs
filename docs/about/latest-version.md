# Latest version and related info

## Latest version of...

!!! important "DS4WINDOWS"

    The currently maintained version of DS4Windows is the one from the **CircumSpector Team**. If you are using any DS4Windows version lower than the currently latest version from CircumSpector it's recommended that you update (Check your current version on DS4Windows' Log tab)

    - [CircumSpector's DS4Windows Github page](https://github.com/CircumSpector/DS4Windows)
        - Make sure to get the latest NON-BETA version from the Release Page
        - The release page contains the changelog
        - **CS's DS4Windows does not support auto-update currently**. Check the instructions below on how to manually update it:

    -----------------

    **Manually updating DS4W:**
    
    === "Step 1"

        1. Make sure DS4Windows is STOPPED AND FULLY CLOSED
            - Make sure it's actually closed and not just "hidden" in the traybar (near Windows' clock)
        1. Download the new version of CS's DS4Windows
        1. Extract it to a **NEW** folder

    === "Step 2"

        1. Open the folder containing the **OLD** version of DS4Windows
        1. **IF** they exist (they might not), copy the following files/folders from the **OLD** DS4Windows folder to the one with the **NEW** version folder:
            - Actions.xml
            - Auto Profiles.xml
            - ControllerConfigs.xml
            - LinkedProfiles.xml
            - OutputSlots.xml
            - Profiles.xml
            - Profiles **folder**

    === "Step 3"

        1. Open the new version of DS4Windows
            - Make sure to confirm in the Log tab that it's actually the new version
        1. If everything seems to be working _OK_, delete the folder of the old version
        1. The end!

??? info "COMPANION DRIVERS (click to expand)"

    These are the drivers used by DS4Windows so it can properly function (for more info on them check the [companion driver's page](../companion-drivers/)). Make sure to check now and then if you have installed the latest version of each:

    - [ViGEm's ViGEmBus](https://github.com/ViGEm/ViGEmBus/releases)
    - [ViGEm's HidHide](https://github.com/ViGEm/HidHide/releases)
        - When updating HidHide, the user must:
            1. Uninstall current version
            1. Reboot
            1. Install latest version
            1. Reboot again
    - Ryochan7's FakerInput v0.1
        - It's installed by DS4Windows itself, so just make sure you are on DS4Windows latest version

## Current state of the DS4Windows project

- The project is alive, being currently maintained by the CircumSpector Team
    - The versions currently being released called starting with "v3" are small bug-fixes on top of the latest Ryochan7's version
    - No major features will be introduced since the whole code is being reworked/modernized. DS4Windows "v4" will have big visual and "under-the-hood" changes once it's released

