
**hardening and securing os x
http://docs.hardentheworld.org/OS/MacOS_10.12_Sierra/
https://github.com/drduh/macOS-Security-and-Privacy-Guide
https://github.com/fix-macosx/yosemite-phone-home/
http://www.macworld.com/article/2048160/how-the-nsa-snoop-proofs-its-macs.html
https://livingthing.danmackinlay.name/osx_hacks.html
https://gist.github.com/guycalledseven/16bdaee3099773865d93

**booting into safemode if you break something**
https://support.apple.com/en-us/HT201573

1. Use these steps to start up your Mac in single-user mode or verbose mode:
2. Shut down your Mac.
3. Press the power button to start up your Mac.
4. Immediately hold down the following keys:
5. Hold down Command-S for single-user mode.
6. Hold down Command-V for verbose mode.


**file locations and useful things to know**

/System/Library/LaunchDaemons/ – System-wide daemons provided by Mac OS X
/System/Library/LaunchAgents/ – Per-user agents provided by Mac OS X
~/Library/LaunchAgents/ – Per-user agents provided by the user
/Library/LaunchAgents/ – Per-user agents provided by the administrator
/Library/LaunchDaemons/ – System-wide daemons provided by the administrator

- launchd manages processes, both for the system as a whole and for individual users using .plist files

https://www.cyberciti.biz/faq/disabling-unnecessary-mac-osx-services/


**1.
https://gist.github.com/mikermcneil/10005651
https://www.jamf.com/jamf-nation/discussions/12694/suppress-yosemite-app-store-notification-via-command

**2.
http://osxdaily.com/2015/05/04/disable-gatekeeper-command-line-mac-osx/

**3.
https://github.com/drduh/macOS-Security-and-Privacy-Guide
http://apple.stackexchange.com/questions/222859/icloud-drive-bird-service-always-running

**4.
http://www.dgkapps.com/blog/osx-tips/osx-tips-turn-off-disable-apple-push-notifications-from-the-command-line/
http://apple.stackexchange.com/questions/92214/how-to-disable-apple-push-notification-service-apsd-on-os-x-10-8

**5.
hardening link

**6.
https://superuser.com/questions/920116/disable-auto-launching-of-photos-application-on-mac-osx-yosemite-el-capitan

**8.
https://discussions.apple.com/thread/5969257?tstart=0

**10.

**11.
https://forums.macrumors.com/threads/question-about-activity-monitor-com-apple-geod-not-responding.1811829/

**12.
https://discussions.apple.com/thread/7025815?start=0&tstart=0

**13.
http://osxdaily.com/2016/12/12/show-user-library-folder-macos-sierra/

**14. disable imagent
http://www.dgkapps.com/blog/osx-tips/osx-tips-turn-off-disable-imagent-from-the-command-line/


**15.
http://www.dgkapps.com/blog/osx-tips/osx-tips-turn-off-disable-bonjour-from-the-command-line/

**16.
How to Disable System Integrity Protection in macOS Sierra
https://www.igeeksblog.com/how-to-disable-system-integrity-protection-on-mac/

**17.
http://apple.stackexchange.com/questions/211062/repeated-crashes-of-suggestd

**18.
https://simon.heimlicher.com/articles/2011/03/17/cisco-vpn-10.6.0-3
