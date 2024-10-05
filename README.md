# Nti-linux-lab5
1.	Attempt to run the command gnuplot. You should find that it is not installed.

2.	Using yum, Search for the plotting packages.

3.	Find out more information about the gnuplot package.

4.	Install the gnuplot package.

5.	Attempt to remove the gnuplot package, but say no

6.	How many packages would be removed

7.	Attempt to remove the gnuplot-common package but say no

8.	How many packages would be removed

9.	Create the file /etc/yum.repos.d/cdrom.repo to enable install from the iso of Red Hat

10.	Using rpm, List all installed packages in your system.

11.	 View the files in the initscripts package

12.	Get general information about bash rpm.

13.	Which installed packages have gnome in their names?

14.	You want to know some information about the status of the system every ten minutes today between the hours of  8:00 AM and 5:00 PM. to help investigate some performance issues you have been having. You suspect it might be memory related and want to keep an eye on those resources.

15.	Use fdisk -l to locate information about the partition sizes.

16.	Use fdisk to add a new logical partition that is 1GB in size.

17.	Did the kernel feel the changes? Display the content of /proc/partitions file? What did you notice? How to overcome that?

18.	Make a new ext3 file system on the new logical partition you just created.

19.	Create a directory, name it /data.

20.	Add a label to the new filesystem, name it data.

21.	Add a new entry to /etc/fstab for the new filesystem using the label you just create.

22.	vi /etc/fstab

23.	Mount the new filesystem.

24.	Display your swap size.

25.	Create a swap file of size 512MB.

26.	Add the swap file to the virtual memory of the system.

27.	Display the swap size.

28.	Use the fdisk command to create 2 Linux LVM (0x8e) partitions using "unpartitioned" space on your hard disk. These partitions should all be the same size; to speed up the lab, do not make them larger than 300 MB each. Make sure to write the changes to disk by using the w command to exit the fdisk utility. Run the partprobe command after exiting the fdisk utility.

29.	Initialize your Linux LVM partitions as physical volumes with the pvcreate command. You can use the pvdisplay command to verify that the partitions have been initialized as physical volumes.

30.	Using only one of your physical volumes, create a volume group called test0. Use the vgdisplay command to verify that the volume group was created.

31.	Create a small logical volume (LV) called data that uses about 30 percent of the available space of the test0 volume group. Look for VG Size and Free PE/Size in the output of the vgdisplay command to assist you with this. Use the lvdisplay command to verify your work.

32.	Create an ext3 filesystem on your new LV.

33.	Make a new directory called /data and then mount the new LV under the /data directory. Create a "large file" in this volume.

34.	Enlarge the LV that you created in Sequence 1 (/dev/test0/data) by using approximately 25 percent of the remaining free space in the test0 volume group.Then, use the ext3 online command to enlarge the filesystem of the LV.

35.	Verify that the file /data/bigfile still exists in the LV. Run the df command and check to verify that more free disk space is now available on the LV.

36.	Use the remaining extents in the test0 volume group to create a second LV called docs. 

37.	Run the vgdisplay command to verify that there are no free extents left in the test0 volume group.

38.	Create an ext3 filesystem on the new LV, make a mount point called /docs and mount the docs LV using this mount point.

39.	Add all of the remaining unused physical volumes that you created in Sequence 1 to the test0 volume group.

40.	If you run vgdisplay again, there now should be free extents (provided by the new physical volumes) in the test0 volume group. Extend the docs LV and underlying filesystem to make use of all of the free extents of the test0 volume group. Verify your actions.

41.	





