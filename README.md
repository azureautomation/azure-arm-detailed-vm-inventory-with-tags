Azure ARM Detailed VM Inventory with Tags
=========================================

            

2017-10-19 - Updated to add Host Caching per disk as well as Availability Zones (Preview)


--------------------------------------------------------------------------


2017-05-20 - Updated to support Azure PS Module 4.0.0 (May 10th update) and added support for Managed Disks


--------------------------------------------------------------------------


2017-02-09 - Removed SubsID and SubsName from Output and Rename all headers to fix an issue where a tag nam conflicted with output header. 


--------------------------------------------------------------------------


2016-12-28 -  Updated to add NIC Provisioning State and fix for Tag Keys case sensitivity


--------------------------------------------------------------------------


2016-12-15 - Updated to add a flag for Single Instance VM under SLA ([https://azure.microsoft.com/en-us/support/legal/sla/virtual-machines/](https://azure.microsoft.com/en-us/support/legal/sla/virtual-machines/))


Single instance VM must have all disks as Premium and must be a xS_ series VM to have a guaranteed uptime of 99.9%.  This can be useful for Production/SQL VMs.  Details can be found in the link above.


--------------------------------------------------------------------------


2016-12-06 - Updated to add VHDs Storage Account settings (Replication and tier (Standard/Premium)


--------------------------------------------------------------------------


Sample script to export detailed configuration of Azure ARM VMs with Tags.  The output allows filtering by Key tag values.  Support up to 15 tags key per subscription.


It will output multiple NICs configuration, as well as Disks if more then one resource exist per vm. 


**Note:** Default output file under c:\temp.  change location at line 58 of the script as needed.


 


 

 



        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
