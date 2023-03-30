# argon2 
## chatgpt 
Argon2 is a command-line utility that performs password hashing using the Argon2 hash function, which is a memory-hard hash function designed to resist attacks from specialized hardware such as ASICs, while also being highly resistant to side-channel attacks. 

The Argon2 command typically takes the following arguments:

- Password: the password that needs to be hashed.
- Salt: a random value that is applied to the password before hashing to prevent pre-computed dictionary attacks.
- Memory cost: the amount of memory that is required during hashing. This value determines the amount of memory that can be used by an attacker’s hardware during a brute force attack.
- Time cost: the number of iterations that are required to perform the hash function. This value determines the amount of time that an attacker must spend to perform a brute force attack.
- Parallelism: the degree of parallelism that is used during hashing. This value determines the number of cores that must be used by an attacker to perform a brute force attack.

Using Argon2 to hash passwords is recommended over other traditional hashing algorithms such as MD5 or SHA1 because of its resistance to attacks like brute force attacks. However, it's also important to ensure that other security measures are in place to protect passwords such as storing them securely and securely transmitting them over networks. 

## tldr 
 
> Calculate Argon2 cryptographic hashes.
> More information: <https://github.com/P-H-C/phc-winner-argon2#command-line-utility>.

- Calculate a hash with a password and a salt with the default parameters:

`echo "{{password}}" | argon2 "{{salt_text}}"`

- Calculate a hash with the specified algorithm:

`echo "{{password}}" | argon2 "{{salt_text}}" -{{d|i|id}}`

- Display the output hash without additional information:

`echo "{{password}}" | argon2 "{{salt_text}}" -e`

- Calculate a hash with given iteration [t]imes, [m]emory usage, and [p]arallelism parameters:

`echo "{{password}}" | argon2 "{{salt_text}}" -t {{5}} -m {{20}} -p {{7}}`
