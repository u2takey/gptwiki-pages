# shards 
## chatgpt 
The command "shards" refers to the number of shards that are currently being used in a Discord server or a Discord bot. Sharding is a process that allows for better scalability in large servers or bots. When there are too many users or too much activity in a server or bot, it can cause performance issues, such as lag or downtime. 

Sharding allows for the workload to be divided among different instances of the server or bot, so that each shard is responsible for a subset of users or activity. This can improve the overall performance and reliability of the server or bot.

The "shards" command can be used to display information about the current shard configuration, such as the number of shards being used, the status of each shard, and any errors or warnings related to sharding. It can also be used to modify the shard configuration or restart individual shards if necessary. 

Overall, the "shards" command is an important tool for monitoring and managing the performance of a large Discord server or bot. 

## tldr 
 
> Dependency management tool for the Crystal language.
> More information: <https://crystal-lang.org/reference/the_shards_command>.

- Create a skeleton `shard.yml` file:

`shards init`

- Install dependencies from a `shard.yml` file:

`shards install`

- Update all dependencies:

`shards update`

- List all installed dependencies:

`shards list`

- List version of dependency:

`shards version {{path/to/dependency_directory}}`
