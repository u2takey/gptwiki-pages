# jhipster 
## chatgpt 
JHipster is a command line tool used to generate web applications with Spring Boot and Angular or React frameworks. When the command 'jhipster' is run, it initiates the JHipster generator which prompts the user with a series of questions regarding the desired configuration and features of their application. The user can choose various options such as the type of authentication, database, frontend framework, and various other options. Based on the user's choices, the generator creates a fully functional web application with the selected features, which can be further customized based on the user's needs. Overall, running the 'jhipster' command is the first step in creating a fully functional web application using JHipster. 

## tldr 
 
> Web application generator using either monolithic or microservices architecture.
> More information: <https://www.jhipster.tech/>.

- Generate a simple full-stack project (monolithic or microservices):

`jhipster`

- Generate a simple frontend project:

`jhipster --skip-server`

- Generate a simple backend project:

`jhipster --skip-client`

- Apply latest JHipster updates to the project:

`jhipster upgrade`

- Add a new entity to a generated project:

`jhipster entity {{entity_name}}`

- Import a JDL file to configure your application (see: https://start.jhipster.tech/jdl-studio/):

`jhipster import-jdl {{first_file.jh second_file.jh ... n_file.jh}}`

- Generate a CI/CD pipeline for your application:

`jhipster ci-cd`

- Generate a Kubernetes configuration for your application:

`jhipster kubernetes`
