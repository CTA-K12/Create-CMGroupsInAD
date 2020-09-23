# Create-CMGroupsInAD

This is a Script that, when run by a scheduled task, retrieve a CSV file from GitHub with the list of available applications in Microsoft Endpoint Configuration Manager. 
It then creates Active Directory groups in 'OU=Software Distribution,', "$rootDN".
This works in conjunction with concept of ConfigMgr collection membership that is based on an query to AD. 
CTA manages many domains so it's not exactly but close to what Anoop C Nair explains in this blog post. https://www.anoopcnair.com/ad-group-based-sccm-collection/

This is script only really useful when you manage a great number of Active Directory forests like we do. If you only mange one you can simple add the group in AD and you are done.
