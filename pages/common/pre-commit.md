# pre-commit 
## chatgpt 
"pre-commit" is a tool used in git for running pre-commit checks on the code changes that you are about to commit. It ensures that the code you are committing adheres to a certain set of standards and quality criteria.

Here is how the "pre-commit" command works:

1. Install the pre-commit tool: First, you need to install the pre-commit tool on your local machine. You can do this by running the following command:

   `pip install pre-commit`

2. Initialize pre-commit: Next, you need to initialize the pre-commit tool in your git repository. You can do this by running the following command:

   `pre-commit install`

3. Configure pre-commit: Once the pre-commit tool is installed and initialized, you can configure it by creating a ".pre-commit-config.yaml" file in the root directory of your project. This file will contain a list of hooks (plugins) that will be run on every pre-commit check. Each hook has a specific command that it runs on your code changes.

   For example, here is a sample ".pre-commit-config.yaml" file that runs two hooks:

   ```
   repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.0.1
     hooks:
     - id: flake8
     - id: trailing-whitespace
   ```

   In this example, we are using two hooks from the pre-commit-hooks repository. The "flake8" hook runs the "flake8" command to check for PEP8 styling errors, and the "trailing-whitespace" hook runs the "grep" command to check for trailing whitespace in your code.

4. Run the pre-commit check: Once your pre-commit config file is set up, you can run the pre-commit check by running the following command:

   `pre-commit run --all-files`

   This command will run all of the hooks specified in your ".pre-commit-config.yaml" file on all of the files that have been changed in your git repository.

If any of the pre-commit checks fail, the commit will be aborted, and you'll need to fix the errors before trying to commit again. This helps to catch issues early on in the development process, ensuring that the codebase is always in a good state. 

## tldr 
 
> Create Git hooks that get run before a commit.
> More information: <https://pre-commit.com>.

- Install pre-commit into your Git hooks:

`pre-commit install`

- Run pre-commit hooks on all staged files:

`pre-commit run`

- Run pre-commit hooks on all files, staged or unstaged:

`pre-commit run --all-files`

- Clean pre-commit cache:

`pre-commit clean`
