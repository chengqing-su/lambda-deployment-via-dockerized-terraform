# AWS Lambda deployment via Dockerized Terraform Demo

This is a demo to deploy aws lambda via Docker.

Here is another demo to show how to deploy aws lambda via local npm and terraform. https://github.com/chengqing-su/lambda-deployment-via-terraform 

## Prerequisites
- Docker
- AWS

## Code structure
```
.
├── README.md
├── auto
│         ├── compile
│         ├── deploy
│         ├── dev-environment
│         └── terraform
├── deployment
│         ├── main.tf
│         ├── outputs.tf
│         └── variables.tf
├── docker-compose.yaml
├── package.json
├── src
│         └── index.ts
├── tree.txt
├── tsconfig.json
└── yarn.lock
 ```
`deployment`: terraform source code.

`src`: aws lambda code.

`auto`: Automation scripts.

## How to deploy
```
export AWS_ACCESS_KEY_ID=<YOUR_AWS_ACCESS_KEY_ID>
export AWS_SECRET_ACCESS_KEY=<YOUR_AWS_SECRET_ACCESS_KEY> 
export AWS_DEFAULT_REGION=<YOUR_AWS_DEFAULT_REGION>

./auto/deploy
```
