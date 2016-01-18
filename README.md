# EMC ECS Service Broker PCF Tile

## Description

*This Project is in a work in progress state*

A BOSH release for the [ECS CF service broker](https://github.com/emccode/ecs-cf-service-broker).
It is based on [BOSH Generic SB Release](https://github.com/cf-platform-eng/bosh-generic-sb-release),
and along with packages for the CF CLI and the broker itself exposes the following BOSH Errands:

* **deploy-service-broker**:  Deploy the broker as a CF app.
* **register-broker**: Register the deployed broker with CF as service broker.
* **destroy-broker**: Deregister and delete the app from CF.

Upon completion, the broker will support dynamic plans, and a PCF Tile which enables the broker to
be configured from the PCF Ops Manager.

## Current Status

Currently, the release builds and runs the app into Cloud Foundry.

## TODOs

* Check that properties are injecting into the errands
* Dynamically generate plans with correct ECS params
* Test PCF Tile deployment
* Test registration & destroy errands
