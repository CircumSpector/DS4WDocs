# DS4Windows silently does not open, crashes, does not start or fails to save settings

## To whom this page does NOT apply

!!! important
    If your DS4Windows opens and starts normally, but then does not detect controllers or fails for another reason then this page is not for you. Take a look at the other troubleshooting pages.

## What to verify fisrt

### Make sure all prerequisites are installed

- Windows 10 / 11
- [Microsoft .NET 5.0 Runtime or higher FOR DESKTOP APPS](https://dotnet.microsoft.com/download/dotnet/5.0/runtime). The Console or Server version will NOT work, and 99% of the users need the x64 package.
- Visual C++ 2015-2019 Redistributable. [x64 for most people](https://aka.ms/vs/16/release/vc_redist.x64.exe) or [x86 for those on 32 bits systems](https://aka.ms/vs/16/release/vc_redist.x86.exe)
- [ViGEmBus](https://vigem.org/projects/ViGEm/How-to-Install/) driver (DS4Windows should offer to install it when it's not detected)
	- The ViGEm driver requires [Visual-C++ 2017 runtime libraries](https://support.microsoft.com/en-us/topic/the-latest-supported-visual-c-downloads-2647da03-1eea-4433-9aff-95f26a218cc0) (most users need the x64 version)
- Microsoft 360 Driver (link inside DS4Windows, already installed by Windows if you've used a 360 controller before)
	- Already installed by default on Windows 10 and 11


### DS4Windows' Log and Windows' Event Viewer

DS4Windows' Log can give important warnings when issues occur. It may be found in 2 different place and, if it exists on both, the most recent one should be inspected:

- In DS4Windows main folder
- In DS4Windows folder inside `%appdata%` (Press ++win+r++, type `%appdata%`, hit OK then check if the DS4Windows folder exists and the presence of the Log file)

Check the dedicated page for [troubleshooting error messages in DS4Windows' Log](../../under-construction).

!!! info "To Do"
	Add more info related to Windows' Event Viewer

### Confirm DS4Windows folder is not write-protected

DS4Windows may be inside a folder that is write-protected, therefore requiring it to be executed with higher privileges to be able to save and edit data. Such folders can be the "Windows" folder, "Program Files" and sometimes even the user Desktop (unlikely, but possible). 

It's recommended to have DS4Windows inside a folder that is known to not require higher-privileges to prevent this issue, like the user's "Documents" or "Downloads" folder.

### Check if User Data is not corruted

The easy way to check this is making sure DS4Windows is not running and then [backing up and erasing all of its User Data](). If erasing the User Data fix the issue but the user wishes to keep some of its old data, it's possible to restore each User Data related file and folder individually until the corrupted file is found, then removing it only.

## Issues that may prevent DS4Windows from running or starting

### "ViGEmBus is not installed" log message when attempting to start DS4Windows

Either ViGEmBus is not installed or DS4Windows is failing to detect it. The ViGEmBus's guides on how to install, verify if its working correctly, uninstall or perform a full clean of everything vigem related can be found on [ViGEmBus' _How to Install/Remove_ page](https://vigem.org/projects/ViGEm/How-to-Install/).

### "_Attempting to start the service winmgmt failed_" or "_Windows Management Interface not found_" messages

If these messages appear on DS4Windows' Log or in Windows' Event View then try to do the "repair Windows installation" fix using a Microsoft Windows installation media. There has been reports that this fixed a problem of DS4Windows app silently doing nothing when launched -issue. Or run WinOS "WMI repository repair" commands. [Repair WinOS WMI repository](https://www.thewindowsclub.com/how-to-repair-or-rebuild-the-wmi-repository-on-windows-10/)

### User is running `MSI Afterburner` and / or `MSI RTSS RivaTuner`

Some users have reported that certain versions of _**MSI Afterburner**_ and _**MSI RTSS RivaTuner**_ apps are not compatible with WPF version of DS4Windows (every version since v2.0).

RTSS prevents DS4Windows app to startup. Try adding DS4Windows.exe file to RTSS application list and set app option as "Application Detection Level=NONE" in RTSS (search issue tickets with these keywords for more information on DS4Windows' Issue Tracker).

### User has the legacy ScpVBus driver installed

The `Scp Virtual Bus Driver` (ScpVBus) is a legacy driver that was used to spawn virtual Xbox controllers. It has been succeeded by the ViGEmBus.

Though DS4Windows should just ignore the ScpVBus, there is a small chance that having it installed along-side the ViGEmBus can lead to issues.

To properly uninstall and remove remaining traces of it from the system, follow the instructions in the [_Manual removal of ScpToolkit residue page_](https://vigem.org/projects/ScpToolkit/ScpToolkit-Removal-Guide/#remove-scp-virtual-bus-driver) starting from the "Remove Scp Virtual Bus Driver" section. 

### Windows is not updated

When everything else fails, update Windows.
