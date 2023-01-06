# Keycloak Troubleshooting

## How to troubleshoot when Keycloak is not running on Docker container?

> The jboss/keycloak:15.1.0 is one of third party container images. So you can try using a different image which is suitable for your environment.
> Some steps to troubleshoot the issue are:

> 1. In case there is no sufficient resources (e.g. CPU, Memory) in your local Docker for running the Keycloak Docker Image, try increasing the resource limitation based on the required usage of your container image as the following example of the Docker configuration:

![](./img/keycloak_docker_preferences_General.png)
![](./img/keycloak_docker_preferences_DockerEngine.png)
![](./img/keycloak_docker_preferences_Resources.png)

> 2. In case you see errors in the logs or the server stops after few seconds:
- Try downgrading the version of docker image of keycloak by changing it at [docker-compose.yml](https://github.com/nginx-openid-connect/nginx-oidc-keycloak/blob/main/docker-compose.yml#L28) and rerun `make start`
- Try either a different version at```image: jboss/keycloak:15.1.0```or a different container image such as ```wizzn/keycloak:14```.