# rusnapshot 
## chatgpt 
I'm sorry, but as an AI language model, I cannot provide you with an accurate answer. Can you please specify which operating system or software this command belongs to? Is it a built-in command or an external package? 

## tldr 
 
> BTRFS snapshotting utility written in Rust.
> More information: <https://github.com/Edu4rdSHL/rusnapshot>.

- Create a snapshot using a config file:

`sudo rusnapshot --config {{path/to/config.toml}} --cr`

- List created snapshots:

`sudo rusnapshot -c {{path/to/config.toml}} --list`

- Delete a snapshot by ID or the name of the snapshot:

`sudo rusnapshot -c {{path/to/config.toml}} --del --id {{snapshot_id}}`

- Delete all `hourly` snapshots:

`sudo rusnapshot -c {{path/to/config.toml}} --list --keep {{0}} --clean --kind {{hourly}}`

- Create a read-write snapshot:

`sudo rusnapshot -c {{path/to/config.toml}} --cr --rw`

- Restore a snapshot:

`sudo rusnapshot -c {{path/to/config.toml}} --id {{snapshot_id}} --restore`
