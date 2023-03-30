# zdb 
## chatgpt 
The "zdb" command is most commonly used on systems running the ZFS (Zettabyte File System) file system, which is a file system developed by Sun Microsystems (now part of Oracle Corporation).

Here is an explanation of the command:

1. Purpose: The "zdb" command is a utility used for debugging and analyzing ZFS storage pools.

2. Syntax: The syntax of the "zdb" command is:

zdb [-ahsy] [-C] [-d] [-m] [-P] [-Q] [-r] [-U] [-v] [-w] [-x] [-z] 

3. Parameters: Below are some of the important parameters that can be used with the "zdb" command:

    -a: Shows information for all ZFS pools on the system.
    
    -s: Shows summary information for the specified pool.

    -d: Shows detailed information for the specified pool.

    -M: Shows information for all ZFS datasets and snapshots.
    
    -t: Shows transaction group information.
    
    -V: Shows version information for ZFS.
    
    -h: Prints out help information.

4. Output: The "zdb" command generates a lot of output, and the actual output generated depends on the specific parameters used. The output can be quite technical and complex, containing information about various aspects of the ZFS pool, such as vdevs, blocks, and datasets.

5. Example: Here is an example of how the "zdb" command might be used:

    zdb -d tank
    
    This command would show detailed information about the "tank" pool, including information about its vdevs, metadata, and data blocks, as well as some transaction group information.

Overall, the "zdb" command is a powerful tool for debugging and analyzing ZFS storage pools, and is frequently used by system administrators and others working with ZFS. 

## tldr 
 
> ZFS debugger.
> More information: <https://manned.org/zdb>.

- Show detailed configuration of all mounted ZFS zpools:

`zdb`

- Show detailed configuration for a specific ZFS pool:

`zdb -C {{poolname}}`

- Show statistics about number, size and deduplication of blocks:

`zdb -b {{poolname}}`
