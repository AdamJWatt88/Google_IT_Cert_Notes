## Resources
[Article on Size Disk](https://technet.microsoft.com/en-us/library/hh148159.aspx)

-   When you right-click to view the properties of a folder, the property sheet includes two values: Size and Size on disk.
-   Size measures the running tally of the file sizes as reported by the Find­First­File function in the WIN32_FIND_DATA.nFile­Size­Low and nFile­Size­High.
-   Size on disk is more complicated; if the drive supports compression and the file is compressed or sparse, the value reported is the compressed size of the file. If the file is neither compressed nor sparse, then the Size on disk is the file size reported by the Find­First­File function rounded up to the nearest cluster.
-   The Size on disk algorithm was originally developed by the Windows 95 team, whose view of the file system world was biased by their MS-DOS background.
-   The recursive directory search doesn't try to filter out file names referring to the same underlying file by means of a hard link.
-   The recursive directory search skips subdirectories if you don't have access to them, and those files won’t be counted in the total folder size.
-   Symbolic links to files count as zero size because the directory entry for symbolic links reports them as having zero size.
-   The values reported by Size and Size on disk are a rough estimate based on the assumption that most files are of the boring variety with no hard links and negligible use of alternate data streams.
-   If you need to keep careful tabs on disk consumption, you’d be better off using a feature like Disk Quotas, whose purpose is to more intelligently track disk consumption.

#course3-module1 