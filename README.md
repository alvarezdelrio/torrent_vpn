# torrent_vpn
https://github.com/qbittorrent/qBittorrent/wiki/How-to-bind-your-vpn-to-prevent-ip-leaks#introduction

Introduction
Many VPNs offer a 'kill-switch' feature designed to block all internet connections if the VPN connection drops, preventing accidental data leaks like your IP address. However, these kill switches can sometimes be unreliable. To add an additional layer of security, you can configure qBittorrent to bind with your VPN. This ensures data can be transferred if and only if your VPN is currently active, which helps prevent data leaks.

The following is a guide to enable this functionality

Procedure
Windows 11
Open the start menu by pressing the windows key, or by clicking on it.
Type into the search bar view network connections and hit ENTER. Alternatively, you can navigate with Control Panel -> Network and Internet -> Network and Sharing Center. This should open up a list of networks such as Ethernet and/or WiFi.
If your VPN is already listed, great! Remember the name of the adapter.
Otherwise, while this window is open, restart your VPN and a new network adapter may appear. This is your VPN.
This adapter may not have an obviously identifiable name at first. You may rename this to whatever you like by right-clicking and selecting 'rename'.
While your VPN is enabled, restart qBittorrent.
Click Tools.
Click Options.
Click Advanced.
Under the Network Interface drop down box, you should select the name of the VPN's adapter from before.
Select Apply.
Restart qBittorrent.
This completes the bind to your VPN. Note that qBittorrent should now only transfer data if your VPN is active. If you're not seeing data being transferred with your VPN active, try restarting qBittorrent.
