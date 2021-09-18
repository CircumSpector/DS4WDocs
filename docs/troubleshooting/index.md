# Troubleshooting tips and general directions

!!! important "Page under-construction!"

## About the troubleshooting section

This page is dedicated to directing users to the information they need to "help themselves". It's asked that users fully read the pages indicated to them, comprehend the information being given and follow the sections carefully when applicable.

Asking for direct support is currently not available. Even if it was, it should be the last option since if an user makes a question about something that already has been answered on the site then they'll probably just be linked right back here. 

## Most common issues and how to solve 

1. DS4Windows silently does not open, crashes or open as normal but then fail to Start everytime the "start" button is pressed followed by a error message on the Log
	- [DS4Windows silently does not open, crashes, does not start or fails to save settings](../troubleshooting/ds4w-does-not-run/)
1. Issues with getting your controller connected via USB or Bluetooth to the computer or to get them recognize by DS4Windows
	- [Controller detection issues](../troubleshooting/ds4w-controller-detection/)
	- [Bluetooth connection issues](../troubleshooting/bt-connection-issues/)
1. DS4Windows detects your controller and appear to function as normal, but games do not detect the controller
	- [Games not recognizing the virtual controller](../troubleshooting/games-controller-detection/)
1. Games detect the controller but it does not behave as expected when playing
	- It usually boils down to: the double input issue was not prevented, the user is using a misconfigured profile or the physical controller itself is faulty 
	- [Controller not behaving correctly in-game](../troubleshooting/misbehaving-controller-ingame/)

## Keyboard and mouse remapping related issues

Check the [_Keyboard & Mouse (KB+M) remapping issues_ page](../troubleshooting/kb-mouse-issues) for the usual issues faced by users and how to solve them.

For help configuring and fine-tuning a profile to have the best possible keyboard and mouse control then you are out of luck as no such guide exists on this site at the moment.

## Other

### Steam and DS4Windows relationship

- Steam and DS4Windows both have what is called "controller remapping" functions. To avoid conflicts, it's recommended that [every Steam controller related option is disabled](../other/under-construction) so only DS4Windows is being used as a remapper
	- Your controller will work as normal in the vast majority of games regardless of Steam's controller related options being disabled
	- A really small amount of Steam games require the usage of Steam's controller options to have working or full DS4 controller support (e.g.: Horizon Zero Dawn). For more information on this, check the [_Steam related information_ page](../troubleshooting/steam-related).
- Steam ignores DS4 or DualSense controllers (real or virtual) if it detects DS4Windows is running on the user system, __which makes no difference for most users as games will still detect the controllers as normal__. The downsides to this Steam behavior are:
	- Real or virtual Playstation controllers won't be able to control the Big Picture interface (emulated Xbox controllers work as normal)
	- There are a few games that require usage of Steam's controller options to have working or full DS4 controller support (e.g.: Horizon Zero Dawn). Because DS4 controllers are ignored, it's not usually possible to use the controller through the required Steam's `Playstation Configuration Support` in those cases
- It's possible to prevent Steam from detecting that DS4Windows is running to workaround the points given above, but doing so can cause remapping conflicts depending on how both of them are configured, specially if the `Playstation configuration support` option is enabled. __As such, this should only be done if absolutely necessary!__ For more information on this, check the [_Running DS4Windows under a custom ".exe" name_ guide](../guides/ds4w-custom-name/) and the [_how to safely use both Steam Input and DS4Windows_ section](../other/under-construction)

### Headphone/mic issues when controller is connected

Check the dedicated [_Headphone or mic related issues_ troubleshooting page](../troubleshooting/audio-related).

## What to do when you've not found the solution to your issue on the site

??? info "To Do"

    __ARE YOU DEFINITELY, 100% SURE THAT THE SITE DOES NOT CONTAIN INSTRUCTIONS ON HOW TO TROUBLESHOOT YOUR PROBLEM?__ Have you fully read the pages that could be related to your problem?

    As it's written on the beginning of this page, if someone appears asking for help to something that already has been properly explained on the site then that person will just be linked right back to it.

    To ask for help, users are welcome to reach us through DS4Windows' Discussion page (not the issue tracker, __DISCUSSIONS!__) as long as the user follows the instructions on the [_How to properlly ask for help_ page](../other/under-construction).