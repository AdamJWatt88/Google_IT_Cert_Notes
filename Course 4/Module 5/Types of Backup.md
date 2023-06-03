-   **Regular backups are important to protect important data**
-   **Full backups** involve making a copy of all data to be backed up, regardless of whether it has been modified or not
-   Full backups can be inefficient for data that doesn't change very often
-  **Differential backups involve backing up only files that have changed or been created since the last full backup**, making them more efficient
-   **Infrequent full backups should still be performed** to avoid tracking and storing too many copies of changing files
-   **Incremental backups are even more efficient than differential backups**, as only the data that's changed in files is backed up
-   **Recovery with incremental backups can be more time consuming**, as the most recent version of backed up data must be reconstructed by integrating the last full backup with each incremental backup that follows
-   **File compression** can be used to save space in backups, but it may take longer to restore data from a compressed backup
-  **RAID arrays** are a method of taking multiple physical disks and combining them into one large virtual disk
-  **RAID arrays are not a backup solution** and do not protect against accidental file deletion or data corruption by malware.

#backups #differential-backups #incremental-backups #data-recovery #RAID-arrays #RAID #course4-module5 