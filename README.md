# Flask webservice 

A dockerized Flask web app which accepts JSON payload and store them into RabbitMQ server. RabbitMQ is deployed
in Kubernetes as a deployment. This details can be found in k8 folders. Here is roughly the steps:

1. Make changes to Flask web app codes
2. Build Docker image of the Flask app based on the Dockerfile
3. Build RabbitMQ service via K8 (Pending todo list!)
4. Build Flask web app deployment and service via K8

## Folders layout

```bash
.                                                                                                                                                                                                                                                                                                                                                                          ├── flask_docker                                                                                                                                                                                                                                                                                                                                                           │   ├── app                                                                                                                                                                                                                                                                                                                                                                │   │   └── main.py                                                                                                                                                                                                                                                                                                                                                        │   ├── data.json                                                                                                                                                                                                                                                                                                                                                          │   ├── docker-compose.yml                                                                                                                                                                                                                                                                                                                                                 │   ├── Dockerfile                                                                                                                                                                                                                                                                                                                                                         │   └── requirements.txt

├── k8                                                                                                                                                                                                                                                                                                                                                                     │   ├── deployments                                                                                                                                                                                                                                                                                                                                                        │   │   ├── flask-deployment.yaml

│   │   └── rmq-deployment.yaml

│   └── services                                                                                                                                                                                                                                                                                                                                                           │       ├── flask-service.yaml

│       └── rmq-service.yaml

└── README.md

```

