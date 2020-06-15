---
title: "Security Guide: Mac OS X 10.14 Mojave"
linkTitle: "Mac OS X"
weight: 2
description: >
  Security guide for Mac OS X

---

{{% pageinfo %}}
This is a placeholder page that shows you how to use this template site.
{{% /pageinfo %}}

## Software Update

### Check for software update

New releases of MacOS contain security fixes not included in older releases.  It is good security practice to run the latest software release.  

MacOS software updates are divided into two phases: 1.) downloading the update, 2.) restarting MacOS to install the update.  Until MacOS is restarted the computer is still running the older release.  

* Launch "System Preferences."
* Click on "Software Update," then wait until macOS has finished checking for a new release. This may take a few minutes.
  * Check *"Automatically keep my Mac up to date."* When checked, the box appears blue with a white checkmark inside it.
  * __If the software is up to date:__ MacOS will provide the message "Your Mac is up to date."  
  * __If the message indicates "A new release is available:"__ follow the prompts to install the new release and restart MacOS.
![macOS Software Update](/assets/macOS/Mojave/macOS-SoftwareUpdate.jpg)
![macOS Software Update - Your Mac is up to date.](/assets/macOS/Mojave/macOS-YourMacisUpToDate.jpg)

### Enable automatic updates

Select "Automatically keep my Mac up to date" to have your Mac install updates automatically.
![macOS Automatically keep my Mac up to date](/assets/macOS/Mojave/macOS-AutoUpdate.jpg)

## Firewall

### Enable firewall

The firewall prevents unauthorized applications, programs, and services from accepting incoming connections.  Accepting unsolicited incoming connections exposes MacOS to network security risks.  To enable Firewall go to:

* Launch "System Preferences."
* Click "Security & Privacy."
* Select the "Firewall" tab from the top.
* Click "Turn on Firewall" button.  When firewall is enabled, the screen reads "Firewall: On" and a green button appears.
![macOS Security & Privacy](/assets/macOS/Mojave/macOS-SecurityPrivacy.jpg)
![macOS Turn on Firewall](/assets/macOS/Mojave/macOS-FirewallOn.jpg)

### Configure Firewall Options

 "Firewall Options" restricts the applications allowed to receive incoming connections.  The most secure configuration is to enable "Block all incoming connections," however this is not practical for most users because it would block incoming calls from Applications like FaceTime or Skype. To configure Firewall Options go to:

* In Security & Privacy, select the "Firewall" tab from the top
* Click the "Firewall Options..." button, a drop down menu will appear.
* In the drop down window:
  * Uncheck "Automatically allow built-in software to receive incoming connections,"
  * Uncheck "Automatically allow downloaded and signed software to receive incoming connections,"
  * Check "Enable stealth mode."
* Click the "OK" button.
![macOS Firewall Options](/assets/macOS/Mojave/macOS-FirewallOptions.jpg)
![macOS Configure Firewall Options](/assets/macOS/Mojave/macOS-ConfigFirewallOptions.jpg)

### Allow or Block incoming connections

In general, personal computers should only make requests to communicate (outbound connections) not receive and respond to connection requests (incoming connections).  Incoming connections should only be necessary for Applications like FaceTime, Skype, AOL Instant Messenger, or Facebook Messenger - these types of applications allow other persons to call or chat.  Incoming connections are not necessary for macOS to function normally, for macOS to startup, or to browse web pages.

A good way to decide whether to Allow or Block an incoming connection, is to think about what you were doing right before the prompt appeared.  If you just opened an Application or were actively using the Application when the prompt occurred, then "Allow" the incoming connection.  If you are NOT actively using the application to communicate or you are not certain, then "Block" the incoming connection.  Do not "Allow" incoming connections from software or services you do not recognize.  MacOS does not require incoming connections to function normally.

## Security & Privacy

### Configure login and password  

"Disable automatic login" and "Require a password."  Requiring authentication prevents persons with physical access to the computer from accessing account data stored on MacOS or data on authenticated websites (including web-based email and social media accounts).

### Application Identity Security

*__Enable "Allow apps downloaded from: App store and identified developers."__*   The bottom section of the General tab configures Application Identity Security.  Application Identity Security prevents a developer from misrepresent who made the software.  For example, Application Identity Security prevents Jarod Smith from claiming his Application was made by Google, Inc. It is good security practice to verify the identity of App developers before permitting their software programs to run.

Enabling apps downloaded from "App store and identified developers" is a trade-off between security and practicality.  Restricting this setting to allow apps downloaded from: "App store" is not practical because many developers choose not to submit their Apps to the App store, since Apple takes a 30% cut when the App is purchased through the App store. To configure, go to:

* Launch "System Preferences."
* Click on "Security & Privacy."
* Select the "General" tab at the top of the window.
  * Check "Require password {5 minutes} after sleep or screensaver," and choose "5 minutes" from the dropdown menu.
  * Check "Disable automatic logins."
  * At the bottom, choose "Allow apps downloaded from: App store and identified developers"
![macOS Disable automatic login](/assets/macOS/Mojave/macOS-SecurityPrivacy.jpg)
![macOS Disable automatic login](/assets/macOS/Mojave/macOS-DisableAutomaticLogin.jpg)
![macOS Allow Apps downloaded from](/assets/macOS/Mojave/macOS-AllowAppsDownloadedFrom.jpg)

*__Enable "Log out after {25 minutes} of inactivity."__* It is good security practice to log out users when the computer is unattended. When MacOS is unattended with a user logged in, any person with physical access to the computer can access data on MacOS or authenticated websites.  

*__Enable "Require an administrator password to access system wide preferences."__*  Changes to "system wide preferences" could compromise the security of MacOS.  Enabling "Require an administrator password to access system wide preferences" protects the system in a situation where someone has gained unauthorized access but does not have the login password of a user with administrator privileges.  It is good security practice to require administrator authentication before allowing updates to security settings. To configure:

* Launch "System Preferences."
* Click "Security & Privacy."
* Select the "General" tab at the top of the window.
* Click the "Advanced" button at the bottom of the window.
  * Check "Log out after {60 minutes} of inactivity," then click the "60" text area and replace with "25."
  * Check "Require an administrator password to access system wide preferences."
![macOS Advanced Security & Privacy](/assets/macOS/Mojave/macOS-GeneralAdvancedSecurityPrivacy.jpg)  
![macOS Advanced Security & Privacy](/assets/macOS/Mojave/macOS-AdminPassToAccessSystemwidePref.jpg)

## FileVault

*__Enable FireVault.__* When FireVault is enabled, files are encrypted with a secret key unique to the User before they are saved to the disk; when FireVault is disabled, files are saved as plain text.  FireVault encrypted files cannot be decrypted and read without access to the secret key.  When a User logs in to MacOS, the disk is decrypted before the desktop loads, it typically takes MacOS an additional 10-20 seconds to decrypt the disk.  It is good security practice to use encryption. To enable FireVault go to:

* Launch "System Preferences."
* Click "Security & Privacy."
* Select the "FireVault" tab at top of the window.
* Click the "Turn on FireVault" button,  a dropdown menu will appear:
  * Choose "Create a recovery key and do not use my iCloud account," click "Continue"
  * After this a new dropdown will appear with the recovery key macOS generated, take a photo of the recovery key or write it down.
  * Click "Continue."
![macOS Turn On FireVault](/assets/macOS/Mojave/macOS-TurnOnFireVault.jpg)
![macOS Turn On FireVault](/assets/macOS/Mojave/macOS-FireVaultCreateRecoveryKey.jpg)
![macOS Turn On FireVault](/assets/macOS/Mojave/macOS-FireVaultRecoveryKey.jpg)

## Users & Groups

### Disable Guest User log in

The "Guest User" login does not require a password. It is good security practice to require Users to authenticate.  To disable Guest User go to:

* Launch "System Preferences"
* Click "Users & Groups"
* Click "Click lock to make changes" at bottom left
  * Enter administrator credentials in the dropdown window
* Click on "Guest User" in the left column.
* Uncheck "Allow guests to log in to this computer."  
  * In the User list (the left column), "Guest User" will now read "Off."
![macOS Users & Groups](/assets/macOS/Mojave/macOS-UsersGroups.jpg)
![macOS Guest User Off](/assets/macOS/Mojave/macOS-UGAllowGuestsToLogintothiscomputer.jpg)

### Disable Automatic Login and Password Hints

*__Set "Automatic Login: Off,"__* because it is good security practice to require Users to authenticate.

*__Disable "Show Password Hints."__*  During MacOS setup, the User is prompted to create a "Password Hint".  Many Users will list their password as the hint.  It’s good security practice to use an external organization method for passwords.  

* Launch "System Preferences"
* Click "Users & Groups"
* Click "Click lock to make changes" at bottom left
  * Enter administrator credentials in the dropdown window
* Click "Login Options" in the left column.
* Next to "Automatic login:" choose "Off" from the dropdown menu.
* Uncheck "Show password Hints"

![macOS Login Options](/assets/macOS/Mojave/macOS-UGShowPasswordHints.jpg)

## Network

*__Disable "Ask to join new networks.__* Joining a new network exposes MacOS to security risks resulting from an absent or misconfigured network security gateway or network firewall.  Computers can be the target of attacks from other computers that share the same network.    It is good security practice to join the fewest number of networks possible.  To disable "Ask to join new networks," go to:

* Launch "System Preferences"
* Click "Network"
* Click "Click lock to make changes" at bottom left.
  * Enter administrator credentials in the dropdown menu
* Uncheck "Ask to join new networks."

![macOS Network](/assets/macOS/Mojave/macOS-Network.jpg)
![macOS Ask to join new networks](/assets/macOS/Mojave/macOS-AskToJoinNewNetworks.jpg)

*__Require administrator authorization to change WiFi network configuration.__*  To configure, go to:

* Launch "System Preferences"
* Click "Network"
* Click "Click lock to make changes" at bottom left
  * Enter administrator credentials in the dropdown window
* Click the "Advanced" button, a dropdown window will appear.
  * Choose the "WiFi" tab at the top of the window
    * Under "Require an administrator authorization to:"
      * Check "Create computer-to-computer networks,"
      * Check "Change networks,"
      * Check "Turn Wi-Fi on or off"

![macOS Network WiFi Require administrator authorization to](/assets/macOS/Mojave/macOS-NetworkRequireAdminAuthTo.jpg)

## Energy Saver

*__Enable "Turn the display off after {10 mins)" and Uncheck "Prevent computer from sleeping automatically when the display is off"__* It is good security practice to log out users when the computer is unattended.

*__Disable "Wake for WiFi network access".__* This setting was created for an environment where computers on the same local network shared files by directly accessing another computer's file system. This is not common today. To configure, go to:

* Launch "System Preferences"
* Click "Energy Saver"
* Select the "Power Adapter" tab from the top.
* Click "Click lock to make changes" at bottom left
  * Enter administrator credentials in the dropdown window.
* Slide the pointer next to "Turn display off after:" until it reads "10 mins"
* Uncheck "Prevent computer from sleeping automatically when display is off"
* Uncheck "Wake for WiFi network access"

![macOS Energy Saver](/assets/macOS/Mojave/macOS-EnergySaver.jpg)
![macOS Energy Saver - Power Adapter](/assets/macOS/Mojave/macOS-ESPowerAdapter.jpg)

We need to configure similar settings for the Battery that we did for the Power Adapter above. *__Enable "Turn the display off after {2 mins}."__*

* Launch "System Preferences"
* Click "Energy Saver"
* Select the "Battery" tab from the top.
* Click "Click lock to make changes" at bottom left
  * Enter administrator credentials in the dropdown window.
* Slide the pointer next to "Turn display off after:" until it reads "2 mins"

![macOS Energy Saver - Battery](/assets/macOS/Mojave/macOS-ESBattery.jpg)

*__Congifure a Schedule to shudown MacOS.__* When macOS is shutdown, the data on the computer is secure, it is good security practice to shutdown macOS whenever the computer is not not actively in use.  Setting an Energy Saver Schedule to automatically shutdown macOS at a specific time is a good way to secure macOS for several hours while the computer is not in use, for instance while the User sleeps.  If a User is still actively using macOS when the Schedule occurs, macOS will prompts the User that the Scheduled activity is about to occur, and the User can interrupt the shutdown. To configure go to:

* Launch "System Preferences"
* Click "Energy Saver"
* Select the "Schedule" button, a dropdown window will appear,
  * Check the second Row
    * In the first box select "Shutdown" from the dropdown menu
    * In the second box select "Everyday"
    * Type "5:30 PM" in the thrid box

![macOS Energy Saver - Schedule](/assets/macOS/Mojave/macOS-ESSchedule.jpg)
![macOS Energy Saver - Schedule - Shutdown Everyday](/assets/macOS/Mojave/macOS-ESShutdownEveryday.jpg)

## General

**_Enable Close windows when quitting an app._** By default macOS preserves a record of the windows that were in use before quitting an Application.  This would allow another person with access to the User account to see what window and files were open the last time the App was used.  Enabling Close windows when quitting an app, macOS will load the application, but not open the windows or files that were last in use.

**_Set Recent Items to None._** Recent Items provides a list of the most recently opened Documents, Apps, and Servers, both from the Finder Window and within specific Applications like Preview > File (menu) > Open Recent.  When "Recent Items" is enabled, macOS is creating a record of your file access history.  It is good security practice to limit the creation of data.

**_Disable handoff_** Handoff uses iCloud to pass data between Applications such as Safari, Calendar, Mail, and some third party Apps. It is good security practice to limit the creation and sharing of data. By using Handoff, you are sharing data about your Application use with iCloud, including Safari browsing history.

* Launch "System Preferences"
* Click "General"
  * Check "Close windows when quitting an app"
  * Next to "Recent Items" select "None" from the dropdown menu
  * Uncheck "Allow handoff between this Mac and your iCloud devices"

![macOS General](/assets/macOS/Mojave/macOS-General.jpg)
![macOS General settings](/assets/macOS/Mojave/macOS-GeneralPane.jpg)

## Spotlight

**_Disable "Spotlight Suggestions"._** The Spotlight Application allows Users to search their local macOS file system using a search prompt instead of clicking through Finder.  Anywhere the Spotlight icon, a magnifying-glass, appears macOS will use the Spotlight search Application.  "Spotlight Suggestions" is a setting within Spotlight search.  When "Spotlight Suggestions" is enabled, macOS shares the text entered into a Spotlight search prompt to Apple who then performs an internet lookup on the users behalf.  It is good security practice to limit the sharing of data.

**_Disable "Allow Spotlight Suggestions in Look up"._**  A "Look Up" is a search for word or phrase using macOS' builtin Dictionary Application. To use "Look Up" the User highlights a word or phrase then opens the Context Menu by Control+Click or Right-click, "Look Up" is the first option the pop-up menu. When "Allow Spotlight Suggestions in Look Up" is enabled, macOS shares the highlighted phrase with Apple in addition to performing a local Dictionary lookup.  It is good security practice to limit the sharing of data.

To disable Spotlight Suggestions:

* Launch "System Preferences"
* Click "Spotlight"
* Select the "Search Results" tab
  * Uncheck "Spotlight Suggestions"
  * Uncheck "Allow Spotlight Suggestions in Look up"

![macOS Spotlight](/assets/macOS/Mojave/macOS-Spotlight.jpg)
![macOS Spotlight Suggestions](/assets/macOS/Mojave/macOS-SpotlightSuggestions.jpg)

## Sharing

*__Disable Sharing services.__* When Sharing Services are off other computers on the same network will be prevented from accessing files and remotely logging in to macOS.  It is good security practice to limit network and file access to macOS.  MacOS Mojave has 9 separate Sharing Services, all of these Services should be turned off. To disable Sharing services go to:

*__Rename the Computer.__* By default, the "Computer Name" is set to something like "User's MacBook."  By identifying the computer as a MacBook anyone on the network who saw the Computer Name would also know the operating system the computer is running, and the username.  It is good security practice to not share information about the operating system or User Accounts with the network.  

* Launch "System Preferences"
* Clikc "Sharing"
* Unckeck all boxes under the "On" column in the table on the left.
* In the text box next to "Computer Name" change the value to a random string that doesn't include the computer make or user name

![macOS Sharing](/assets/macOS/Mojave/macOS-Sharing.jpg)
![macOS Sharing Services Off and Rename Computer](/assets/macOS/Mojave/macOS-SharingServicesOffComputerName.jpg)

## AirDrop

**_Disable AirDrop._**  AirDrop allows macOS to send and receive documents, photos, websites, contacts, map locations and other files to nearby devices running macOS or iOS.  When AirDrop is enabled, other macOS or iOS devices can determine the  relative location of the computer (via Bluetooth and WiFi), and other computer can send files to macOS.  It is good security practice to not share location and to not allow other computers to send files to macOS.  To disable AirDrop go to:

* Launch "Finder," which can be found in the Dock
* Click "AirDrop" in the left column (If AirDrop is not present in the left column see below) &rarr;
* Click "Allow me to be discovered by:" at the bottom of the window
  * select "No One" from the dropdown menu

![macOS Finder icon in Doc](/assets/macOS/Mojave/macOS-DockFinder.jpg)
![macOS Finder AirDrop Discovered By No One](/assets/macOS/Mojave/macOS-FinderAriDropDiscoveredByNoOne.jpg)

**_If AirDrop is not present in the Finder Window, use these steps to make AirDrop visible._**  

* Open Finder
* On the file menu click "Finder," at the upper left corner of the screen
  * Click "Preferences" from the dropdown menu
  * Choose the "Sidebar" tab at the top of the "Finder Preferences" window
    * Check AirDrop under the "Favorites" section,
* Then return to the Finder window and continue disabling AirDrop as shown above.

![macOS Finder File Menu Preferences](/assets/macOS/Mojave/macOS-FinderFileMenuPreferences.jpg)
![macOS Finder Preferences Sidebar AirDrop](/assets/macOS/Mojave/macOS-FinderPreferencesSidebarAirDrop.jpg)

## Firmware Password

Firmware provides the interface between macOS and the physical hardware on the MacBook (processors, displays, harddrives, network interfaces, memory and more).  MacOS uses the industry standard UEFI command language (Universal Extensible Firmware Interface).  Most hardware vendors produce hardware that can interpret and respond to UEFI commands.

Setting a firmware password prevents  modification to PRAM firmware.  A firmware password prevents macOS from being booted from an external drive (such as a USB drive).  The firmware password is required before macOS will boot into recovery mode.

The process to set a firmware password involves restarting macOs twice, and usually requires about 8-10 minutes.  Take a photo or lookup the instructions on another device before attempting to set a firmware password.  

1. Shutdown macOS and then start up macOS in "macOs Recovery mode."  To startup in "macOS Recovery mode" press hold Command (⌘)-R and immediately after turning on the Mac.  Release the keys after the Apple logo appears.  It typically takes macOS longer to start up in "macOS Recovery mode" than to boot into normal mode (between 3-5 minutes).
1. The macOS Utilities screen will appear.  Click on "Utilities" in the file menu.  Then click on "Startup Security Utility" from the dropdown window.
![macOS Firmware Startup Security Utility](/assets/macOS/Mojave/macOS-StartupSecurityUtility.jpg)
1. Click the "Turn On Firmware Password" button.
![macOS Firmware Turn On Firmware Password](/assets/macOS/Mojave/macOS-FirmwarePassOff.jpg)
1. Enter the new firmware password in the drop down window that appears.  Then click the "Set Password" button.
![macOS Firmware Enter a new firmware password](/assets/macOS/Mojave/macOS-EnterFirmwarePasswordjpg.jpg)
1. After the firmware password is accepted, the message "Firmware password protection enabled." will appear.  Click the "Quit Startup Security Utility" button.
![macOS Firmware password protection enabled](/assets/macOS/Mojave/macOS-FirmwarePasswordProtectionEnabled.jpg)
1. Click the Apple Logo () in the upper left hand corner. Then click "Restart" from the dropdown menu for the firmware password to take effect.
![macOS Firmware restart for password to take effect](/assets/macOS/Mojave/macOS-Utilities-Restart.jpg)