# in-toto-run 
## chatgpt 
The `in-toto-run` command is used in the in-toto framework, which is a security-minded tool used to ensure the integrity of software supply chains. Here's a detailed explanation of the command:

Command name: `in-toto-run`

Syntax: `in-toto-run [OPTIONS] [Metablock PATH] [STEP NAME] [COMMAND]`

Description of each parameter:

- `OPTIONS`: Optional additional arguments that can be passed to `in-toto-run`. These may include things like specifying a different key to use for signing, or overriding the expiration date of the resulting Metablock.
- `Metablock PATH`: The path to a Metablock file that defines a series of steps in the software supply chain. `in-toto-run` executes a single step within this chain, and generates a new Metablock to prove that the step was executed as intended.
- `STEP NAME`: The name of the step to execute within the defined supply chain. This should match the name of a step defined in the Metablock.
- `COMMAND`: The command to execute for this step. This should be a shell command that will be executed within the current environment.

Functionality: When `in-toto-run` is executed, it performs several actions:

1. It checks that the specified Metablock file exists and is readable.
2. It extracts the specified step from the Metablock file.
3. It checks that the step has not already been executed (by checking the `byproducts` section of the Metablock).
4. It executes the specified command within the current environment.
5. It generates a new Metablock that proves that the step was executed correctly. This Metablock will be signed with the private key associated with the specified step, and will include information about the input files, output files, and command executed for this step.

Once the `in-toto-run` command has completed, you will have a new Metablock file that proves that the specified step was executed correctly, along with a chain of trust back to the original key used to sign the first Metablock. This can be used to ensure the security and integrity of your software supply chain, and to provide evidence that your software has not been tampered with at any point during the process. 

## tldr 
 
> Generating link metadata while carrying out a supply chain step.
> More information: <https://in-toto.readthedocs.io/en/latest/command-line-tools/in-toto-run.html>.

- Tag a git repo and signing the resulting link file:

`in-toto-run -n {{tag}} --products {{.}} -k {{key_file}} -- {{git tag v1.0}}`

- Create a tarball, storing files as materials and the tarball as product:

`in-toto-run -n {{package}} -m {{project}} -p {{project.tar.gz}} -- {{tar czf project.tar.gz project}}`

- Generate signed attestations for review work:

`in-toto-run -n {{review}} -k {{key_file}} -m {{document.pdf}} -x`

- Scan the image using Trivy and generate link file:

`in-toto-run -n {{scan}} -k {{key_file}} -p {{report.json}} -- {{/bin/sh -c "trivy -o report.json -f json <IMAGE>"}}`
