# PADL Base
Default Base image for PADL Bridge application.
Consists of an LTS linux image (Ubuntu 22.04) with:
- OpenLdap
- OpenJDK 11 LTS
- Creation of an application user - ```padl```
- ```sudo``` configuration for some administrative requirements for ```padl``` user

## Building 

```bash
# Docker
docker build https://github.com/xandecelo/padlbase.git#main  -t alefzero/padlbase

# Openshift CLI
oc new-app https://github.com/xandecelo/padlbase.git#main --name=alefzero/padlbase

```