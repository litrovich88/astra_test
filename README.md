# astra_test
Test task for AstraLinux

## Overview
Here's a quick start demo stack for Prometheus and Grafana with 1860 dashboard in Docker containers. The dashboard configured to view vagrant box metrics from Prometheus node exporter.
## Requirements

- Vagrant app
- Vagrant box Ubuntu 20.04 with name 'ubuntu2004'
- Virtualization app (ex. VirtualBox)

## Run
Go to the project directory and run 'vagrant up' for first run. Next time run 'vagrant up --provision' (without it ansible playbooks will not applied). You can access to http://localhost:3000 in browser when command is done. Login to Grafana with admin/admin, skip password change (it will not be saved after restart).

## Content
- config directory with docker-composer.yml, Prometheus and Grafana configs
- ansible playbooks: setup (it runs playbooks for configuring box), docker (install docker and docker compose), node_exporter (install node exporter on box host) and up_ct (run containers by docker-compose)

