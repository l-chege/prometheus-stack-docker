# Prometheus Observability Stack SetUp Using Docker
DevOps Tools used:
- Docker
- Prometheus
- Alert Manager
- Grafana
- Prometheus Node Explorer
- Terraform and AWS EC2 services. 

Linux concepts covered as part of setup:
- Makefile - used to modify the server IP address in prometheus configuration.
- Linux SWAP - to add swap to the ec2 instance.
- Shell scripts - to install docker, docker compose and add swap as part of ec2 system startup.

## Prerequisites
To deploy prometheus stack on docker, ensure you have the following:
- AWS account with a key pair/value.
- AWS CLI configured with the account.
- Terraform installed on local machine.


## Installation
- Provision ec2 using terraform
- Deploy prometheus stack using docker compose
- Validate prometheus node exporter metrics
- Configure grafana dashboards
- Configure node exporter dashboard 
- Simulate & test alert manager alerts - test high storage & cpu alert  

