# redis-cli 
## chatgpt 
The redis-cli command is a command-line interface utility for Redis, an in-memory data structure store that is often used as a database, cache or message broker. The redis-cli utility allows users to communicate with Redis from a terminal application or shell. 

When the redis-cli command is executed, it opens an interactive shell where users can issue commands and receive responses from the Redis server. Redis commands are composed of a command name followed by a series of arguments. These commands can be issued directly from the redis-cli prompt, or they can be batched and executed from within a script file. 

Some examples of Redis commands that can be executed using redis-cli include:

- SET: sets a value for a given key
- GET: retrieves the value of a given key
- DEL: deletes a given key and its associated value
- KEYS: lists all keys stored in Redis
- INCR: increments the value of a given key
- EXPIRE: sets a timeout for a given key

With the redis-cli command, users can also configure Redis settings, monitor Redis activity, and interact with Redis pub/sub channels. 

Overall, the redis-cli utility is a powerful tool for managing Redis instances and working with Redis data. 

## tldr 
 
> Opens a connection to a Redis server.
> More information: <https://redis.io/topics/rediscli>.

- Connect to the local server:

`redis-cli`

- Connect to a remote server on the default port (6379):

`redis-cli -h {{host}}`

- Connect to a remote server specifying a port number:

`redis-cli -h {{host}} -p {{port}}`

- Connect to a remote server specifying a URI:

`redis-cli -u {{uri}}`

- Specify a password:

`redis-cli -a {{password}}`

- Execute Redis command:

`redis-cli {{redis_command}}`

- Connect to the local cluster:

`redis-cli -c`
