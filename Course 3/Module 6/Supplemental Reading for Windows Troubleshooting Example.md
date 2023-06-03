
## Troubleshooting a problem in Windows

As an IT Support professional, you will likely run into problems caused by a full primary hard drive, where the OS is installed. An affected computer may display an error message stating there is insufficient space on the drive to save new files, apply an update, or install new software. In some cases, the computer might not provide an informative error message at all. Instead, the system may experience performance issues, hang, crash, or it might not even load the OS after booting. Note that it is a best practice to routinely perform maintenance and clean-up of computer hard drives to free storage space, improve system performance, and prevent the myriad of issues that can arise when the primary hard drive is full.

Imagine that you are an IT Support Specialist for an organization. An employee reports that their computer is running very slowly and keeps hanging. You know that Windows Update had been scheduled to run overnight to update all of the organization’s systems with multiple patches, updates, and fixes. Although it is possible for these changes to cause system problems, there is only one employee reporting a problem. So, it is more likely that the system did not have adequate storage space to install all of the updates on that employee’s computer system. You suspect that the primary hard drive could be full. Your troubleshooting and repair steps might include:

1.  **Check how much free storage space remains.** A quick and easy troubleshooting step for system performance issues is to check if the primary hard drive is full. In this scenario, you discover that the employee’s hard drive has less than 5 GB of space left. Microsoft recommends giving Windows 10 at least 20 GB of free space for normal OS processes. You will need to find at least 15 GB of files to delete or move to another storage location. 
    
2.  **Delete temporary and unneeded files.** There are a few methods for cleaning out junk files from Windows. Two system maintenance tools for this purpose, found in several versions of Windows, include:
    
    1.  **Storage Sense:** Use the Windows Storage Sense tool to delete unnecessary files like temporary files, offline cloud files, downloads, and those stored in the Recycle Bin. You can also configure Storage Sense to regularly and automatically clean the hard drive for proactive maintenance. 
        
    2.  **Disk Cleanup:** A simple alternative tool to Storage Sense. Disk Cleanup performs most of the same operations as Storage Sense, plus it offers a drive compression utility. Note: If you run Disk Cleanup on a drive, but the computer is still reporting “Low Disk Space”, the Temp folder is most likely filling up with Microsoft Store .appx files. In this case, you will need to clear the cache for Microsoft Store.
        
3.  **Reset Windows Update.** Since you know the employee’s computer went through a Windows Update overnight and possibly did not complete this process fully, it may be wise to perform a Windows Update reset. The reset tool can check whether a system reboot is required to apply the updates, security settings were changed, update files are missing or corrupted, service registrations are missing or corrupt, and more.This utility can be found in the Windows system **Settings** menu, under **Troubleshoot > Other troubleshooters >  Windows Update**.
    
4.  **Move files off of the primary hard drive and onto** (one or more of the following)**:** 
    
    1.  **Internal or external storage device:** Install an additional hard drive or add an external storage device, like a USB drive or SD card, to hold user files.
        
    2.  **Network storage:** Network storage space is often available in network environments in the form of Network Attached Storage (NAS) appliances or large Enterprise Storage Area Networks (SANs). In these environments, end users should have network drive space mapped to their workstations for file storage, instead of saving files to their local hard drives. 
        
    3.  **Cloud storage** (OneDrive, File Explorer, Google Drive, etc.)**:** Providing cloud storage space to end users is a lower cost alternative to network storage. However, this option is less secure than onsite NAS or SAN storage.
        

In Windows **System Storage**, under **Advanced storage settings**, set the new drive storage as the destination for “Where new content is saved.”   

1.  **Set any cloud storage** **solutions to be online-only.** This will prevent cloud files from downloading an offline or cached version of the files to the hard drive. 
    
2.  **Uninstall apps that are not needed** (including Windows Store apps)**.** This is an effective way to free up large amounts of storage space. 
    
3.  **Run antivirus and antimalware software.** Some viruses and malware intentionally fill up hard drives with garbage data.
    
4.  **Wipe hard drive and reinstall the OS.** If none of the suggestions listed above solve the problem with slow system performance and hanging, consider wiping the hard drive and reinstalling the OS. This is the best method for repairing failed system updates.
    

## Resources

-   [Free up drive space in Windows](https://support.microsoft.com/en-us/windows/free-up-drive-space-in-windows-85529ccb-c365-490d-b548-831022bc9b32#WindowsVersion=Windows_10) - Microsoft article for Windows 10 and 11 that provides step-by-step instructions for freeing storage space on a hard drive. 
    
-   [Low Disk Space error due to a full Temp folder](https://support.microsoft.com/en-us/windows/low-disk-space-error-due-to-a-full-temp-folder-8eb375af-c5d4-22ac-3f3a-ac0a98382749#ID0EDD=Windows_10) - Steps to clear the cache for Microsoft Store and reset Windows Update for Windows 10 and 11.
    
-   [Manage drive space with Storage Sense](https://support.microsoft.com/en-us/windows/manage-drive-space-with-storage-sense-654f6ada-7bfc-45e5-966b-e24aded96ad5) - Instructions for configuring this Windows tool to automatically remove temporary files, downloads, offline cloud files, and empty the Recycle Bin.
    
-   [How to use Event Viewer on Windows 10](https://www.windowscentral.com/how-use-event-viewer-windows-10) - A walkthrough tour of Windows Event Viewer with screenshots and detailed explanations of each part of the tool.
    
-   [How do I reset Windows Update components?](https://docs.microsoft.com/en-us/windows/deployment/update/windows-update-resources) - Steps for troubleshooting problems with Windows Update.