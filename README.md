## avro-deserialization

In order to run the example after importing it in Anypoint Studio, you will need to :
1. Update the src\main\resources\config-dev.yaml with the appropriate connection properties to Kafka cluster and Confluent schema registry URL.
2. Add the Kafka keystore "dev-imd-kaas.keystore.jks" & the truststore "dev-kaas-truststore.jks" to the src\main\resources folder of the example project.
3. Update the src\main\resources\config-secured-dev.yaml file with the encrypted secrets for Kafka keystore and truststore. Refer [Securing Config Props](https://docs.mulesoft.com/mule-runtime/4.4/secure-configuration-properties#secure_props_tool) for encryption process in case needed.
4. Run the project with arguments -Dmule.env=dev and -Dmule.encryptionKey=<Used for encryption>
