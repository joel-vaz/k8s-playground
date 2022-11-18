## Summary 
Introduction demo using Mongo DB

## Description

1. 2 Deployments
2. 2 Services
3. 1 Config Map
4. 1 Secret

## Details

1 Internal Service on MongoDB - No external requests.

ConfigMap: DB URL
Secret: DB User, DB Pwd

1 Mongo express deployment.

1 External Service - allow external requests

browser -> Mongo Express / External Service -> Mongo Express -> Mongo DB/Internal Service (connects using ConfigMap and Secret) -> MongoDB 

Terminal: $ echo -n "username" | base64

## Instructions

$kubectl apply -f mongo-secret.yaml

