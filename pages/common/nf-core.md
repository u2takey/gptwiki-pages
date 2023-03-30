# nf-core 
## chatgpt 
The command "nf-core" refers to a command-line tool used in bioinformatics workflows. The "nf" stands for Nextflow, which is a popular workflow management system used to execute complex computational pipelines in a reproducible and scalable way.

"nf-core" is a collection of pre-built, community-curated Nextflow workflows for a variety of bioinformatics applications, such as genomics, transcriptomics, proteomics, and others. These workflows have been optimized and validated to work on a variety of computing platforms, from laptops to high-performance computing clusters. The nf-core command allows users to easily download, configure, and execute these workflows on their own data.

When executed, the "nf-core" command lists available workflows from a central repository, and the user can select a workflow for their specific application. The command then downloads the workflow and associated configuration files, and provides instructions on how to configure the workflow for the user's specific input data.

Overall, the nf-core command simplifies the process of setting up and executing complex bioinformatics data analysis workflows, allowing researchers to focus more on their research and less on computational infrastructure. 

## tldr 
 
> The nf-core framework tools, to create, check and develop best-practice guidelines for Nextflow.
> More information: <https://nf-co.re/tools>.

- List existing pipelines on nf-core:

`nf-core list`

- Create a new pipeline skeleton:

`nf-core create`

- Lint the pipeline code:

`nf-core lint {{path/to/directory}}`

- Bump software versions in pipeline recipe:

`nf-core bump-version {{path/to/directory}} {{new_version}}`

- Launch an nf-core pipeline:

`nf-core launch {{pipeline_name}}`

- Download an nf-core pipeline for offline use:

`nf-core download {{pipeline_name}}`
