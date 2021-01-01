# config-repo-service
configuration details for all APIs


TO RUN THE PROGRAM:

## In ECLIPSE

1. add an environment variable by name "ENCRYPT_KEY" and provide the value of encryption key used.
2. pass this variable to program arguments

example : {ENCRYPT_KEY}

adding variable:

![variable](https://github.com/API-Demonstration-Project-1/config-repo-service/blob/master/env_variable_in_eclipse.jpg)

passing the variable as an argument:

![argument](https://github.com/API-Demonstration-Project-1/config-repo-service/blob/master/program_argument.png)

## In Console

java -jar config-repo-service.jar XYZENCRYPTIONKEY

----------------------------------------------------------------


## What is ready?

  - a working spring boot app
  - dockerized
  - properties encrypted
  - secured using SSL with HTTPS

## Pending:

- authentication 
- mavenizing docker image creation
- CI/CD