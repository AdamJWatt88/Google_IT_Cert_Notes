-   **Swap space** is a dedicated area of the hard drive used for **virtual memory**
-   To create swap space, we can use the new disk partitioning tools we learned
-   A good guideline for determining how much swap space is needed is to follow the recommended partitioning scheme
-   We can create swap partitions for main storage devices like hard drives and SSDs
-   To create a **swap partition**, go back into the **parted tool** and select the drive to partition
-   Create a **partition** using the command `mkpart primary linux-swap 5Gib 100%`
-   To complete the process run the `quit` command to exit parted, run the make swap command `sudo mkswap /dev/sda2` on the new swap partition, then enable swap on the device with `sudo swapon /dev/sda2`. 
-   To automatically mount swap space every time the computer boots up, add a swap entry to the `/etc/fstab` 

# Supplemental Reading for Linux Swap

For more information about _swap_, please check out the link [here](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/storage_administration_guide/ch-swapspace).

#linux #swap-space #swap-partition #course3-module4 