# Homeassistant Kubernetes YAML

This repository contains YAML resources to deploy Homeassistant on Kubernetes. 

The deployment leverages the container that is maintained by the Homeassisant project. 

[https://github.com/home-assistant/core/pkgs/container/home-assistant](https://github.com/home-assistant/core/pkgs/container/home-assistant)

Deployment manages updates via the `stable` tag against the latest stable Homeassistant release. 

Updates can be done simply by deleting the running Pod instance. The `Deployment` Pod spec contains the `imagePullPolicy: Always` definition. 