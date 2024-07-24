
## Créer un réseau

```shell
    docker network create applications-network
```

## Créer un répertoire pour les configurations

```shell
    mkdir -p /opt/tools/jenkins
```

## Droits du répertoire

```shell
    chmod ugo+rwx -R  /opt/tools/jenkins
```

## Exécution

```shell
    cd /opt/tools/ci-cd/jenkins
    docker compose up -d
    docker exec -it jenkins-jdk17 cat /var/jenkins_home/secrets/initialAdminPassword
```


## Mot de passe administrateur

```shell
    docker exec -it jenkins-jdk17 cat /var/jenkins_home/secrets/initialAdminPassword
```

## Actions

- Installer les plugins suggérés
- Créer un utilisateur

