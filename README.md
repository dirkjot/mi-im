# mi|im -- Mirror Image

### Problem
You want to share a dashboard or CI board which is hosted inside a VPN with collaborators that are not on the VPN.  Or you want to share a dashboard with your colleages for use on their personal devices, without having to install VPN on those. 

### Solution
`mi|im` provides a two-part solution:
1. Install a node.js script inside the firewall, which takes regular screenshots of the dashboard using pageres
2. Install `mi|im` on your PAAS of choice (it was made with CloudFoundry in mind) and have the node.js upload the screenshots there

Now, you can point a regular browser at the secured endpoint of `mi|im` to get regular updates on the dashboard.

