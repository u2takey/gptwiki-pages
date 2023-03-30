# nextflow 
## chatgpt 
Nextflow is a command-line tool and a domain-specific language (DSL) used for building and executing high-throughput computational pipelines. It is designed to facilitate the creation of complex, scalable, and reproducible workflows for big data and distributed computing environments.

The 'nextflow' command is used to run Nextflow workflows. When executed, the Nextflow engine interprets the DSL script specified by the user, creates a dependency graph of the workflow, and executes the steps of the workflow in parallel on a local machine, a multi-cloud infrastructure, or a high-performance computing cluster.

The 'nextflow' command can be used with various options and arguments to customize the execution of the workflow, such as:

- 'run' option to specify the path to the main Nextflow DSL script
- 'with-report' option to enable the generation of an HTML report of the workflow execution
- 'resume' option to resume a previous workflow execution from a checkpoint
- 'run' argument to pass parameters to the workflow execution (e.g., input files, output files, configuration values)

Nextflow also provides several other commands, such as 'init', 'config', 'pull', and 'log', to initialize a new workflow project, configure the Nextflow environment, update the Nextflow version, and view the workflow execution logs, respectively. 

Overall, the 'nextflow' command is essential for running and managing Nextflow workflows, and it provides a flexible and powerful framework for building and executing reproducible and scalable data analysis pipelines. 

## tldr 
 
> Tool for running computational pipelines. Mostly used for bioinformatics workflows.
> More information: <https://www.nextflow.io>.

- Run a pipeline, use cached results from previous runs:

`nextflow run {{main.nf}} -resume`

- Run a specific release of a remote workflow from GitHub:

`nextflow run {{user/repo}} -revision {{release_tag}}`

- Run with a given work directory for intermediate files, save execution report:

`nextflow run {{workflow}} -work-dir {{path/to/directory}} -with-report {{report.html}}`

- Show details of previous runs in current directory:

`nextflow log`

- Remove cache and intermediate files for a specific run:

`nextflow clean -force {{run_name}}`

- List all downloaded projects:

`nextflow list`

- Pull the latest version of a remote workflow from Bitbucket:

`nextflow pull {{user/repo}} -hub bitbucket`

- Update Nextflow:

`nextflow self-update`
