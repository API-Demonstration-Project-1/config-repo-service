# config-repo-service
configuration details for all APIs

<p>
All the configurations for apps such as
  tenant management service
  authentication jwt service etc
are available through this service(config-repo-service)
</p>


This service is available at the url - https://localhost:8888/.
Because this is available as an HTTPS service the certificate must be added to JVM so that other services can access the HTTPS url when running on local system.

Use the below command to add proarchs certificate to JVM's cacerts


> keytool -import -trustcacerts -alias proarchskeystore -file /path/to/file/proarchscert.cer -keystore ${JAVA_HOME}/jre/lib/security/cacerts -storepass changeit

The certificate file is available at the root of the project as a .p12 file.


======

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

