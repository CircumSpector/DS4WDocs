# Companion drivers

## General info

To properly function or to have its capabilities improved, DS4Windows makes use of first and third-party drivers, some of which are required while others are optional. This page contains a list of all drivers that were currently or previously associated to it.  

## Required and optional drivers

### Nefarius' Virtual Gamepad Emulation Bus (Nefarius' ViGEmBus)

The ViGEmBus driver is the most important driver used by DS4Windows. It can create virtual/fake/emulated controllers, which DS4Windows uses to spawn virtual Xbox and DS4 controllers.

### Nefarius' HidHide

The HidHide driver allows the user to "hide" gamepads from the system and make them detectable to only chosen programs in order to prevent the infamous [double input issue](../../guides/solving-double-input/).

### Travis Nickles' FakerInput

DS4Windows uses the FakerInput driver to expose system-wide virtual keyboard, relative mouse and absolute mouse. Allows Keyboard + Mouses events/commands to be usable in some situations where the usual way DS4Windows sends those commands (via "SendInput) fails. Examples of those situations are elevated processes and games, UAC prompts and anti-cheat systems that block SentInput events. Use of FakerInput is necessary to allow DS4Windows to work with some games with anti-cheat protection like valorant.

## Legacy drivers

### Nefarius' HidGuardian

HidGuardian is a driver that can hide controllers from the system and allow only chosen processes to detect them. It was previously used by DS4Windows to solve the double input issue, but was made obsolete by the release of its successor, HidHide, a similar driver that works better and is easier to use.

DS4Windows removed support for HidGuardian in version 3.0.8 in favor of HidHide. As such, users who used and still have HidGuardian installed can be in a state where their controllers are hidden and undetectable to Windows and DS4Windows.

**It's highly recommended for the user to follow [HidGuardian's uninstall instructions](../../guides/uninstalling-ds4windows/#legacy-drivers) in order to verify if it's installed and how to safely remove it in case it is.**

### Virtual Gamepad Emulation Bus (ScpVBus)

!!! note "Necessary to confirm the information here"

The ScpVBus driver is used to create fake/virtual/emulated Xbox 360 controllers. It was made obsolete by the release of its successor, the ViGEmBus driver.

Usually, users accidentally install this driver when they search for "DS4Windows" on google and end-up clicking on the first result that appears, which leads to the original (but now obsolete) version of DS4Windows from the developer Jays2kings which prompts the user to install it. 

ScpVBus is not used anymore by Ryochan7's DS4Windows besides for experimenting purposes on special testing builds. Therefore, this driver has no use for the average user and [it's better if it were to be uninstalled in case it's present](../../guides/uninstalling-ds4windows/#legacy-drivers) since it has a minor chance of causing issues/BSoD on Windows.
