# molecule 
## chatgpt 
Molecule is a command-line tool used for developing, testing, and deploying Ansible roles. It is designed to simplify the process of building, testing, and distributing roles for Ansible. 

Molecule can be used for test-driven development (TDD), where test cases are written first and then code is developed to pass these tests. This helps to ensure that the code is working as expected and avoids the need for manual testing.

Some common commands used with Molecule are:

1. molecule init - This command creates a new role directory structure with a basic template and directory structure.

2. molecule create - This command creates the test environment in which the role will be tested.

3. molecule converge - This command applies the role to the test environment.

4. molecule verify - This command runs the tests, which can be either the default tests included with Molecule or custom tests defined by the user.

5. molecule destroy - This command removes the test environment.

Overall, Molecule is a powerful tool for automating the development and testing of Ansible roles, and helps to ensure high-quality code that is easily deployable. 

## tldr 
 
> Molecule helps testing Ansible roles.
> More information: <https://molecule.readthedocs.io>.

- Create a new Ansible role:

`molecule init role --role-name {{role_name}}`

- Run tests:

`molecule test`

- Start the instance:

`molecule create`

- Configure the instance:

`molecule converge`

- Log in into the instance:

`molecule login`
