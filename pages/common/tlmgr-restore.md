# tlmgr restore 
## chatgpt 
The command "tlmgr restore" is a command used in TeX Live Manager, a software used for installing, updating, and managing TeX packages in a TeX Live distribution. This command is used to restore the previous state of the TeX distribution to a specific date by installing or uninstalling packages.

When executed, tlmgr restore will provide a list of backups or snapshots of the TeX Live installation, sorted by date. The user can choose the date they want to restore their TeX Live installation to by entering the corresponding number.

After the user selects the date they want to restore to, tlmgr will remove any packages that were installed after that date and install any packages that were removed or updated since that date. This will restore the TeX Live distribution to its exact state as it was on the chosen date.

The tlmgr restore command can be helpful in cases where a recent package update or installation causes issues in the TeX Live compilation process. Restoring to a previous state can help to isolate the problematic package and troubleshoot the issue. 

## tldr 
 
> Restore package backups created with `tlmgr backup`.
> The default backup directory is specified by the `backupdir` option, and can be obtained with `tlmgr option`.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- List all available backup revisions for all packages:

`tlmgr restore`

- List all available backup revisions for a specific package:

`tlmgr restore {{package}}`

- Restore a specific revision of a specific package:

`tlmgr restore {{package}} {{revision}}`

- Restore the latest revision of all backed-up packages:

`tlmgr restore --all`

- Restore a package from a custom backup directory:

`tlmgr restore {{package}} {{revision}} --backupdir {{path/to/backup_directory}}`

- Perform a dry-run and print all taken actions without making them:

`tlmgr restore --dry-run {{package}} {{revision}}`
