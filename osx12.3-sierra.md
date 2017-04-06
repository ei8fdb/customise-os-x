
**1. disable notification centre**
launchctl unload -w /System/Library/LaunchAgents/com.apple.notificationcenterui.plist
killall NotificationCenter

or
sudo defaults write /System/Library/LaunchAgents/com.apple.notificationcenterui KeepAlive -bool false
Killall NotificationCenter

**2. kill appstore gatekeeper**
sudo spctl --master-disable
spctl --status

**3. disable, and turn-off all icloud**
sudo defaults write NSGlobalDomain NSDocumentSaveNewDocumentsToCloud -bool false

sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.icloud.findmydeviced.plist
sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.cloudfamilyrestrictionsd-mac.plist

sudo launchctl unload -w /System/Library/LaunchAgents/com.apple.cloudd.plist 
launchctl unload -w /System/Library/LaunchAgents/com.apple.cloudd.plist 

sudo launchctl unload -w /System/Library/LaunchAgents/com.apple.icloud.findmydeviced.findmydevice-user-agent.plist
launchctl unload -w /System/Library/LaunchAgents/com.apple.icloud.findmydeviced.findmydevice-user-agent.plist

sudo launchctl unload -w /System/Library/LaunchAgents/com.apple.icloud.fmfd.plist
launchctl unload -w /System/Library/LaunchAgents/com.apple.icloud.fmfd.plist

sudo launchctl unload -w /System/Library/LaunchAgents/com.apple.cloudpaird.plist
launchctl unload -w /System/Library/LaunchAgents/com.apple.cloudpaird.plist

sudo launchctl unload -w /System/Library/LaunchAgents/com.apple.bird.plist
launchctl unload -w /System/Library/LaunchAgents/com.apple.bird.plist

sudo launchctl unload -w /System/Library/LaunchAgents/com.apple.bird.plist
launchctl unload -w /System/Library/LaunchAgents/com.apple.bird.plist

**4. disable apple push notifications**
sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.apsd.plist
ps aux | grep apsd
sudo launchctl list | grep apsd

**5. disable OS X sending diag information to Apple
sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.SubmitDiagInfo.plist
sudo launchctl list | grep DiagInfo

**6. disable photos opening when plugging in a photo device**
defaults -currentHost write com.apple.ImageCapture2 HotPlugActionPath ''
defaults -currentHost write com.apple.ImageCapture disableHotPlug -bool YES
defaults -currentHost write com.apple.Photos disableHotPlug -bool YES

**7. disable photos related agents
sudo launchctl unload -w /System/Library/LaunchAgents/com.apple.cloudphotosd.plist
launchctl unload -w /System/Library/LaunchAgents/com.apple.cloudphotosd.plist

**8. disable location services
sudo launchctl unload /System/Library/LaunchDaemons/com.apple.locationd.plist
launchctl unload -w /System/Library/LaunchDaemons/com.apple.locationd.plist

sudo launchctl unload /System/Library/LaunchAgents/com.apple.maspushagent.plist
launchctl unload -w /System/Library/LaunchAgents/com.apple.maspushagent.plist

**9. disblae iphone related agents and services
sudo launchctl unload /System/Library/LaunchAgents/com.apple.CallHistoryPluginHelper.plist
launchctl unload -w /System/Library/LaunchAgents/com.apple.CallHistoryPluginHelper.plist

sudo launchctl unload /System/Library/LaunchAgents/com.apple.CallHistorySyncHelper.plist
launchctl unload -w /System/Library/LaunchAgents/com.apple.CallHistorySyncHelper.plist

**10. disable games centre
sudo launchctl unload /System/Library/LaunchAgents/com.apple.gamed.plist
launchctl unload -w /System/Library/LaunchAgents/com.apple.gamed.plist

**11. disable geod service**

**12. disable mapspush daemon**
sudo launchctl unload /System/Library/LaunchAgents/com.apple.maspushagent.plist 
launchctl unload -w /System/Library/LaunchAgents/com.apple.maspushagent.plist

**13. unhide ~/Library/ directory**
chflags nohidden ~/Library/

**14. disable imagent
launchctl unload -w /System/Library/LaunchAgents/com.apple.imagent.plist
sudo launchctl list | grep imagent



**15. disable bonjour service**
sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.mDNSResponder.plist
sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.mDNSResponderHelper.plist
sudo launchctl list | grep mDNS
