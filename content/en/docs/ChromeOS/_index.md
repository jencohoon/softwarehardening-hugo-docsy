---
title: "Security Guide: Chrome OS 76"
linkTitle: "ChromeOS"
weight: 2
description: >
  Security guide for Chrome OS

---

## Software Update
  
Every new release of Chrome OS contains security fixes not included in older releases.  It is good security practice to run the latest software release.  

ChromeOS software updates are divided into two phases: 1.) downloading the update, 2.) restarting ChromeOS to install the update.  Restarting is necessary for the update to take effect.  Until ChromeOS is restarted the computer is still running the older release.  To update go to:

Settings &rarr; click "About Chrome OS" from the list on the left (if no list is visible on the left, click the hamburger menu next to Settings at the top of the window) &rarr; click the "Check for updates" button

If the message reads "Your Chromebook is up to date" no action is required.  If the message indicates "A new release is available", follow the prompts to install the new ChromeOS release and restart.

![ChromeOS Settings Hamburger](/assets/ChromeOS/76/webfiles/ChromeOS-Settings-hamburger.png)
![ChromeOS About Chrome OS](/assets/ChromeOS/76/webfiles/ChromeOS-AboutChromeOS.png)
![ChromeOS Check for Software Update](/assets/ChromeOS/76/webfiles/ChromeOS-AboutChromeOS-CheckforUpdate.png)
![ChromeOS Software Update Your Chromebook is up to date](/assets/ChromeOS/76/webfiles/ChromeOS-AboutChromeOS-YourChromebookIsUptoDate.png)

## Bluetooth

*__Consider turning Bluetooth off.__*  It is good security practice to disable unused services such as Bluetooth. Some external computer accessories rely on Bluetooth, such as speakers, headphones,  mouse, or keyboard.  To  check if any devices are connecting to ChromeOS using Bluetooth, click the word "Bluetooth," and check if any devices are listed under "Paired Devices." If no devices are listed, then it is alright toggle off Bluetooth.   To turn off Bluetooth go to:

Settings &rarr; Bluetooth &rarr; click the arrow next to "Bluetooth"

* &rarr; In the Bluetooth window under "Paired Devices" check for listed devices. The "Paired Devices" listing will only appear if Bluetooth is currently set to ON.
* &rarr; If no "Paired Devices" are listed, toggle off at the top.  When correctly set the toggle reads "Off."
![ChromeOS Bluetooth On](/assets/ChromeOS/76/webfiles/ChromeOS-Bluetooth-On.png)
![ChromeOS Bluetooth Check for Paired Devices](/assets/ChromeOS/76/webfiles/ChromeOS-Bluetooth-PairedDevices.png)
![ChromeOS Bluetooth Off](/assets/ChromeOS/76/webfiles/ChromeOS-Bluetooth-Off.png)

## People

![ChromeOS People Settings](/assets/ChromeOS/76/webfiles/ChromeOS-People.png)

*__Customize Sync settings.__*  It is good security practice to limit the creation and sharing data. Google creates database records for each "Sync" item enabled.  
*__Enable "Settings" syncing__* to preserve *some of the User's ChromeOS settings.*  Synced settings are applied when the User logs into ChromeOS on new computer hardware. To configure, go to:

Settings &rarr; People &rarr; Sync

* &rarr; toggle off Apps
* &rarr; toggle off Bookmarks
* &rarr; toggle off Extensions
* &rarr; toggle off History
* &rarr; toggle on Settings
* &rarr; toggle off Themes & Wallpapers
* &rarr; toggle off Open Tabs
* &rarr; toggle off Passwords
* &rarr; toggle off Addresses, phone numbers, and more
* &rarr; toggle off Payments and addresses using Google Pay

![ChromeOS People Sync custom settings](/assets/ChromeOS/76/webfiles/ChromeOS-People-Sync-CustomSettings.png)

*__Enable "Show lock screen when waking from sleep."__* It is good security practice to log out of User accounts when the computer is unattended.  This prevents persons with physical access to the computer from accessing account data on authenticated websites (including web-based email and social media accounts) and data on the local ChromeOS file system.   To configure, go to:

Settings &rarr; People &rarr; click "Screen lock and sign-in"

* &rarr; provide the password
* &rarr; toggle on "Show lock screen when waking from sleep"
![ChromeOS People Screen Lock and Sign-In](/assets/ChromeOS/76/webfiles/ChromeOS-People-ScreenLockandSignIn.png)

*__Disable Guest browsing__* and *__Restrict sign-in.__* It is good security practice to manage which User accounts are able to log in to a computer. Guest browsing does not require a password. When Guest browsing is enabled, anyone with physical access to the computer can use ChromeOS.  Restricting sign-in fixes which Users can login to ChromeOS.  New Users must be added to the sign-in list by an existing Administrative User.  To configure go to:

Settings &rarr; People &rarr; click "Manage other people"

* &rarr; toggle off "Enable Guest browsing"
* &rarr; toggle on "Restrict sign-in to the following users."  The accounts listed below the setting will be able to login to ChromeOS.
![ChromeOS Manage Other People](/assets/ChromeOS/76/webfiles/ChromeOS-People-ManageOtherPeople.png)

## Autofill

![ChromeOS Autofill](/assets/ChromeOS/76/webfiles/ChromeOS-Autofill.png)

*__Passwords: toggle off "Offer to save passwords" and "Auto Sign-in."__* It is good security practice not to share passwords with third parties.  When "Offer to save passwords" is enabled, the Chrome Web Browser will offer to save passwords; saved passwords are associated with the User's Google Account. When Auto Sign-in is enabled, the Chrome Web Browser will save both the username and the password.  With Auto Sign-in enabled, anyone with access to the User's account on ChromeOS can use the stored credentials to access personal web accounts. To configure, go to:

Settings &rarr; Autofill &rarr; click "Passwords"

* &rarr; toggle off "Offer to save passwords"
* &rarr; toggle off "Auto sign-in"
![ChromeOS Autofill Passwords](/assets/ChromeOS/76/webfiles/ChromeOS-Autofill-Passwords.png)

*__Payment methods: toggle off "Save and fill payment methods."__*  It is good security practice to limit the creation and sharing data. "Save and fill payment methods" creates a copy of payment information (such as credit card information).  To configure, go to:

Settings &rarr; Autofill &rarr; click "Payment methods" &rarr; toggle off "Save and fill payment methods"
![ChromeOS Autofill Payment Methods](/assets/ChromeOS/76/webfiles/ChromeOS-Autofill-PaymentMethods.png)

*__Addresses and more: toggle off "Save and fill addresses."__*  It is good security practice to limit the creation and sharing data. "Save and fill addresses" creates copies of addresses, phone numbers, and email addresses. To configure, go to:

Settings &rarr; Autofill &rarr; click "Addresses and more" &rarr; toggle off "Save and fill addresses"
![ChromeOS Addresses and More](/assets/ChromeOS/76/webfiles/ChromeOS-Autofill-AddressesAndMore.png)

## Device

*__Power: "When idle sleep" and "Sleep when lid is closed."__*  It is good security practice to log out of User accounts when the computer is unattended. Power settings, that cause ChromeOS to enter sleep mode,work together with People settings to prevent access to User data when ChromeOS is unattended.  To configure, go to:

Settings &rarr; Device &rarr; click "Power"

* &rarr; next to "When idle" choose "Sleep" from the drop down menu
* &rarr; toggle on "Sleep when lid is closed"
![ChromeOS Device](/assets/ChromeOS/76/webfiles/ChromeOS-Device.png)
![ChromeOS Device Power](/assets/ChromeOS/76/webfiles/ChromeOS-Device-Power.png)

## Search engine

*__Update "Search engine used in address bar:" DuckDuckGo. and make DuckDuckGo the default search engine__*  It is good security practice to limit the creation and sharing of data. The search engines run by Google, Bing, and Yahoo! save User search history and browsing history (websites visited).  The DuckDuckGo Search Engine does not save User search or browsing history.  To configure go to:

Settings &rarr; Search engine

* &rarr; next to "Search engine used in the address bar" choose "DuckDuckGo" from the dropdown menu
* &rarr; click "Manage search engines"
* &rarr; under "Default search engine" find "DuckDuckGo"
* &rarr; click the three vertical dots on the far right of the DuckDuckGo row,  
* &rarr; choose "Make default" from the popup menu.  When configured correctly, (Default) will appear under DuckDuckGo.
![ChromeOS Search Engine used in Address Bar](/assets/ChromeOS/76/webfiles/ChromeOS-SearchEngine-AddressBar.png)
![ChromeOS Manage Search Engines](/assets/ChromeOS/76/webfiles/ChromeOS-SearchEngine-ManageSearchEngines.png)

## Google Play Store

*__Turn off Google Play Store.__*  Google Play Store is only available on some types of hardware.  If settings for Google Play Store are not found on your ChromeOS device, skip this section.  

It is good security practice to run the least number of services and software programs necessary. Google Play Store allows Android Apps to run within ChromeOS. Turning on Google Play Store exposes ChromeOS to security vulnerabilities present in Android OS and to security vulnerabilities present in any Android Apps that are running. To Turn off Google Play Store go to:

Settings &rarr; Google Play Store &rarr; ensure the button next to "Google Play Store" at reads "Turn On"
![ChromeOS Google Play Store off](/assets/ChromeOS/76/webfiles/ChromeOS-GooglePlayStore.png)

## Linux

*__Turn off Linux.__*  It is good security practice to run the least number of services and software programs necessary.  Turning on Linux enables ChromeOS to run software and services that are disabled when Linux is turned off.    If a service or software program isn't running, it can not be compromised. To configure go to:

Settings &rarr; Linux (Beta) &rarr; ensure the button next to "Linux" at reads "Turn On"
![ChromeOS Linux off](/assets/ChromeOS/76/webfiles/ChromeOS-Linux.png)

## On startup

*__Open the New Tab page on startup__*  It is good security practice to limit the creation and sharing of data.  When "Open a New Tab" is selected, ChromeOS does not create a record of tabs open in Chrome Web Browser, or home pages.  To configure go to:

Settings &rarr; On startup &rarr; select the radio button next to "Open a New Tab page"
![ChromeOS On startup open a new tab](/assets/ChromeOS/76/webfiles/ChromeOS-OnStartup-NewTab.png)

## Privacy and security

Most of the disabled Privacy and security settings share data with Google or third parties. It is good security practice to limit the creation and sharing of data.  The settings discussed below are either enabled to improve security, or affect unrelated ChromeOS services.  

*__Enable: "Safe Browsing (protects you and your device from dangerous sites)."__*  Safe browsing enables the search engine equivalent of a website virus scanner.  When Google's Web Spiders crawl the web to create a search index, Google also checks websites for known malicious software and phishing.  When Google discovers a website contains malicious content, the site is added to a list of unsafe sites.  When Safe Browsing is enabled, Google checks URLs the browser is accessing against it's list of unsafe sites.  If the site appears in the list, Google will warn the User instead of loading the site.

*__Enable: Send a "Do Not Track" request with your browsing traffic.__* It is good security practice to limit the sharing of data. This setting causes ChromeOS to send a "Do Not Track" request to websites you visit; there is no enforcement of this request.

*__Disable: "Help improve Chrome security."__*  ChromeOS has not addressed important security considerations for crash reports, such as: the encryption method used to transmit data, what data is sent, and who has access to the data.  Because the implementation is undefined, sending in crash reports could leak data.  Other operating systems allow Users to review crash reports before sending the crash report.  ChromeOS does not provide this transparency.

*__Disable: "Enable Verified Access."__* The "Verified Access" service is unnecessary for personal use. It is good security practice to disable unused services.  "Verified Access" is an enterprise setting for ChromeOS used by systems administrators responsible for configuring multiple Chrome OS devices on a company network.  "Verified Access" enables access to an API that companies use to configure and verify Chrome OS devices remotely.  

*__Disable: "Keep Wi-Fi on during sleep."__* It is good security practice to disable services when the computer is unattended.  When a Chrome OS is disconnected from all networks, the only way to compromise it is through physical access to the computer.  Network attacks are far more common than attacks involving physical access to a computer's hardware.

To configure Privacy and Security, go to:
Settings &rarr; Advanced &rarr; Privacy and Security

* &rarr; toggle off "Use a prediction service to help complete searches and URLs typed in the address bar or the app launcher search box"
* &rarr; toggle off "Use a web service to help resolve navigation errors"
* &rarr; toggle on "Safe Browsing (protects you and your device from dangerous sites)"
* &rarr; toggle off "Help improve Chrome security"
* &rarr; toggle off "Automatically send diagnostic and usage data to Google"
* &rarr; toggle off "Use enhanced spell check"
* &rarr; toggle on "Send a "Do Not Track" request with your browsing traffic"
* &rarr; toggle off "Allow sites to check if you have payment methods saved"
* &rarr; toggle off "Use a prediction service to load pages more quickly"
* &rarr; toggle off "Enable Verified Access"
* &rarr; toggle off "Keep Wi-Fi on during sleep"
![ChromeOS Privacy and Security](/assets/ChromeOS/76/webfiles/ChromeOS-PrivacyAndSecurity.png)

### Site Settings: Cookies

Site Settings is a menu within the Privacy and Security section.
![ChromeOS Site Settings within Privacy and Security section](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings.png)

*__Cookies: Toggle on "Allow sites to save and read cookie data."__* Blocking Cookies is not practical.  Most everyone uses a web-based email client or online account management for credit cards or utilities, all these services use cookies to allow authenticated access to account information.  

*__Cookies: Toggle on "Keep local data only until you quit your browser."__* The Chrome Web Browser cannot be quit while Chrome OS is running.  Because of this, local cookie data is deleted when Chrome OS is shutdown. Deleting cookies limits the sharing of data.

*__Cookies: Toggle on "Block third-party cookies."__*  It is good security practice to limit the creation and sharing data. Most websites include references to content on third-party sites. That content request could be a request to a third-party server to set and or read cookies on the local Chrome Web Browser.  By blocking third-party cookies, only sites whose URL matches the domain visited by the User are able to set and read cookies.

To configure Cookies go to: Settings &rarr; Advanced  &rarr; Privacy and Security &rarr; click "Site Settings" &rarr; click "Cookies"  

* &rarr; toggle on "Allow sites to save and read cookie data."  
* &rarr; toggle on "Keep local data only until you quit your browser"
* &rarr; toggle on "Block third-party cookies."
![ChromeOS Site Settings Cookies](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-Cookies.png)

### Site Settings: Location

*__Toggle Location to "Blocked."__*  It's good security practice to limit the sharing of data, blocking requests will limit sharing.  Blocking websites from prompting the User to access their location, prevents location data from leaking.

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "Location"  

* &rarr; toggle off "Ask before accessing."  When correctly set the toggle reads "Blocked."
![ChromeOS Site Settings Location blocked](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-Location.png)

### Site Settings: Notifications

*__Toggle Notifications to "Blocked."__*  It is good security practice to silence unimportant messages to prevent alarm fatigue.  By default ChromeOS allows websites, apps or extensions to send the User notifications whenever they want.  Attention to detail is important when running a secure operating system or browsing the web safely.  Distraction like Notifications, make it harder to pick out the details that concern security.

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "Notifications"

* &rarr; toggle off "Ask before accessing."  When correctly set the toggle reads "Blocked."
![ChromeOS Site Settings Notifications blocked](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-Notifications.png)

### Site Settings: Flash

*__Block sites from using Flash.__*  It is good security practice to disable Flash. The Flash Player also called Flash plugin has many known security vulnerabilities. Several web browsers disable Flash by default.  To configure:

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "Flash"

* &rarr; toggle off "Block sites from using Flash."  When correctly set the toggle reads "Block sites from using Flash."
![ChromeOS Site Settings Flash blocked](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-Flash.png)

### Site Settings: Pop-ups and Redirects

*__Block pop-ups and redirects.__*  Pop-up windows and site redirects are the most common attacks on compromised sites.  A site is compromised when it's owner has lost control of site content.  Blocking pop-ups and redirects protects the User from malicious behavior. To configure:

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "Pop-ups and redirects"

* &rarr; toggle off so the message reads "Blocked."
![ChromeOS Site Settings Pop-ups and Redirects blocked](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-PopUpsAndRedirects.png)

### Site Settings: Ads

*__Block Ads on sites that show intrusive or misleading ads.__*  It is good security practice to silence unimportant messages, like intrusive ads, to prevent alarm fatigue.

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "Ads"

* &rarr; toggle off so message reads "Blocked on sites that show intrusive or misleading ads."
![ChromeOS Site Settings Ads](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-Ads.png)

### Site Settings: Background Sync

*__"Do not allow recently closed sites to finish sending and receiving data."__*   Important security details about Background Sync are unknown, such as the metric is used to determine when the site has "finished sending and receiving data" and what safeguards the background sync network connection so it is not exploited.  Disabling Background Sync will not have a negative impact on ChromeOS as tcp, the networking protocol that underlies http(s), elegantly closes network connections.

Background Sync was intended to save the User headache when the network connection was poor. Recognizing the network connection is poor and then choosing not to execute sensitive transactions, such as payment processing or emailing, over unstable networks is more effective at preventing User anxiety.

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "Background Sync"

* &rarr; toggle off so message reads "Do not allow recently closed sites to finish sending and receiving data"
![ChromeOS Site Settings Background Sync](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-BackgroundSync.png)

### Site Settings: Automatic downloads

*__"Do not allow any site to download multiple files automatically."__*  It is good security practice to manage files and to keep only necessary files. Pausing to acknowledge a download provides time to verify the file is needed. Disabling Automatic downloads may interrupt website based peer-to-peer file sharing.  

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "Automatic downloads"

* &rarr; toggle off so message reads "Do not allow any site to download multiple files automatically"
![ChromeOS Site Settings Automatic Downloads](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-AutomaticDownloads.png)

### Site Settings: Unsandboxed plugin access

*__"Do not allow any site to use a plugin to access your computer."__* It is good security practice to maintain process isolation and run software with the lowest privileges necessary.  A unsandboxed process has greater runtime permissions and runs in a shared environment; As opposed to a sandboxed process which runs in an isolated environment with lower permissions.  
ChromeOS is in the process of removing all plugins.  The last widely supported plugin, Adobe Flash, is scheduled to be removed at the end of 2020.  

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "Unsandboxed plugin access"

* &rarr; toggle off so message reads "Do not allow any site to use a plugin to access your computer"
![ChromeOS Site Settings Unsandboxed Plugin Access](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-UnsandboxedPluginAccess.png)

### Site Settings: Handlers

*__Do not allow any site to handle protocols.__*  It is good security practice to silence unimportant messages to prevent alarm fatigue.  Any website can request to become the default protocol handler, then each time the protocol url is clicked that website will load.   Many malicious sites use the tactic of asking the User allow the website to become the default Home Page, Search Engine, etc.  Blocking sites from asking to handle protocols protects ChromeOS from malicious behavior and protects the User from alarm fatigue.

The "protocols" envisioned are the "mailto:" protocol and the "webcal:" protocol, but any protocol could be used. Important security considerations are not addressed in the implementation.

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "Handlers"

* &rarr; toggle off so message reads "Do not allow any site to handle protocols"
![ChromeOS Site Settings Handlers](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-Handlers.png)

### Site Settings: USB  

*__Do not allow any site to access USB devices.__*   It is good security practice to limit the creation and sharing of data. Connecting a website to a USB device lets the website control and record information from the USB device.  The site can copy all the information on the device and can even reprogram it. To configure:

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "USB"

* &rarr; toggle off so message reads "Do not allow any site access USB devices"
![ChromeOS Site Settings USB](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-USB.png)

### Site Settings: PDF documents

*__Disable "Download PDF files instead of automatically opening them in Chrome.__*"  It is good security practice to actively manage files and only keep necessary files.  By opening PDF files in Chrome, the PDF is treated as a cached-file associated with the web browser.  Cached-files are less permanent than downloaded files.  Cached-files can be deleted by choosing to "Clear browsing data" through the Chrome Web Browser.

PDF security vulnerabilities are well documented. The Chrome Web Browser contains a builtin PDF viewer that opens PDF files in a sandboxed environment within Chrome. (This means the PDF files are opened in an isolated process environment.)  The PDF viewer builtin to the web browser is the most compelling security reason to use the Chrome browser. To configure, go to:

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "PDF documents"

* &rarr; toggle off "Download PDF files instead of automatically opening them in Chrome."
![ChromeOS Site Settings PDF Documents](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-PDFDocuments.png)

### Site Settings: Clipboard

*__Do not allow sites to see text and images copied to the clipboard.__*  It is good security practice to limit the creation and sharing data. Disabling clipboard prevents sites from proactively reading clipboard data.  It does not prevent the User from copy and pasting data from the clipboard into the web browser. To configure:

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "Clipboard"

* &rarr; toggle off so message reads "Do not allow sites to see text and images copied to the clipboard."
![ChromeOS Site Settings Clipboard](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-Clipboard.png)

### Site Settings: Payment Handlers

*__Do not allow any site to install payment handlers.__* It is good security practice to carefully consider all the circumstances before allowing any installation.  Payment through websites uses https, an encrypted protocol.  When purchasing from major vendors, like Amazon, or using payment intermediaries like PayPal or Visa Checkout, payment is sent over https.  Because current payment tools are adequate and do not require installation, no compelling security reason exists to install a payment handler.

Settings &rarr; Advanced &rarr; Privacy and Security &rarr; Site Settings &rarr; click "Payment Handlers"

* &rarr; toggle off so message reads "Do not allow any site to install payment handlers."
![ChromeOS Site Settings Payment Handlers](/assets/ChromeOS/76/webfiles/ChromeOS-SiteSettings-PaymentHandlers.png)

## Languages and input

*__Set Spell check to "Basic spell check."__* It is good security practice to limit the creation and sharing of data.  The "Enhanced spell check" option sends the text you type in the browser to Google.  To configure:

Settings &rarr; Advanced &rarr; Languages and input &rarr; under "Spell check:" choose "Basic spell check"
![ChromeOS Languages and Input Basic Spell Check](/assets/ChromeOS/76/webfiles/ChromeOS-LanguagesAndInput-SpellCheck.png)

## Downloads

*__Toggle on "Ask where to save each file before downloading."__*  It is good security practice to manage files and to keep only necessary files. Pausing to acknowledge the download location provides an opportunity to verify the file or program is needed.

Settings &rarr; Advanced &rarr; Downloads &rarr; toggle on "Ask where to save each file before downloading"
![ChromeOS Downloads Ask where to save each file before downloading](/assets/ChromeOS/76/webfiles/ChromeOS-Downloads-AskWhereToSaveEachFile.png)

## Extensions

*__Manage Chrome extensions.__* It is good security practice to run the least number of services and software programs necessary.  Seven Chrome Extensions, listed below, are part of the operating system and will be installed by default on ChromeOS.  All other Chrome Extensions and Apps should be removed.  The Chrome Web Browser is used to manage extensions. To configure:

Open the Chrome Web Browser

* &rarr; manually type chrome://extensions in the address bar.  External sites are prevented from accessing pages starting with "chrome:"
* &rarr; remove all Extensions and Apps not installed by default. The Apps shown below are installed by ChromeOS: Google Docs Offline, Calculator, Docs, Google Keep, Sheets, Slides, and Text.
![ChromeOS Shelf Chrome Web Browser](/assets/ChromeOS/76/webfiles/ChromeOS-Shelf-ChromeBrowser.png)
![ChromeOS Extensions](/assets/ChromeOS/76/webfiles/ChromeOS-Exttensions.png)
