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
