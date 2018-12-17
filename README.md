# springconfig-client
example project for getting config values using spring cloud config

Open bootstrap.properties

spring.cloud.config.uri - should be set to the springcloud config server endpoint

spring.application.name - should match the prefix of the config files in git

spring.profiles.active - should match the suffix of the config files in git

After building and running the project the config values can be retrieved calling the REST endpoint:

curl http://localhost:8777/msg
