# Monitoring-Tools

Liste des outils pour le monitoring des applications

## Configurer le driver docker
- Indentifier le processeur

```sh
dpkg --print-architecture
```
- Installer le driver

```sh
docker plugin install grafana/loki-docker-driver:3.3.2-amd64 --alias loki
--grant-all-permissions
```

-restart le service docker

```sh
sudo systemctl restart docker
```