# lvextend 
## chatgpt 
lvextend is a command used in Linux operating systems to increase the size of a Logical Volume (LV). Logical Volumes are logical partitions created from Physical Volumes (PV) in the Linux LVM (Logical Volume Manager) system.

The lvextend command syntax is as follows:

lvextend [options] Logical_Volume_Path [Physical_Volume_Path]

Here is a brief explanation of the command options:

- -r: This option is used to extend the file system in the Logical Volume automatically after it is extended.
- -L: This option is used to specify the new size of the Logical Volume. For example, lvextend -L +10G Logical_Volume_Path will increase the size of the Logical Volume by 10GB.
- -l: This option is used to specify the new size of the Logical Volume in extents. For example, lvextend -l +100%FREE Logical_Volume_Path will increase the size of the Logical Volume to use all available free space on all of its Physical Volumes.

Here is an example of how to use the lvextend command:

Assuming we have a Logical Volume called /dev/vg1/lv1 mounted on the /data directory with a size of 20GB.
 
1. Check the current size of the Logical Volume:
$ sudo lvdisplay /dev/vg1/lv1
2. Add a new Physical Volume to the Volume Group (VG) that contains the Logical Volume, then scan for the new Physical Volume:
$ sudo pvcreate /dev/sdb1
$ sudo vgscan
3. Extend the Logical Volume by 10GB:
$ sudo lvextend -L +10G /dev/vg1/lv1
4. Check the new size of the Logical Volume:
$ sudo lvdisplay /dev/vg1/lv1
5. Resize the file system to use the newly added space:
$ sudo resize2fs /dev/vg1/lv1

After executing these commands, the Logical Volume will now have a size of 30GB and the file system on it will have been resized to use the newly added space. 

## tldr 
 
> Increase the size of a logical volume.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvextend.8.html>.

- Increase a volume's size to 120 GB:

`lvextend --size {{120G}} {{logical_volume}}`

- Increase a volume's size by 40 GB as well as the underlying filesystem:

`lvextend --size +{{40G}} -r {{logical_volume}}`

- Increase a volume's size to 100% of the free physical volume space:

`lvextend --size {{100}}%FREE {{logical_volume}}`
