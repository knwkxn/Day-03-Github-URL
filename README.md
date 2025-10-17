# LLMSecOps Workshop

This repository implements an end-to-end LLM Security & Operations (LLMSecOps) setup.

## Features
- FastAPI + HuggingFace question-answering model
- Dockerized app
- Vulnerability scanning using Trivy
- Kubernetes deployment manifests

## Run locally
```bash
pip install -r app/requirements.txt
python app/main.py
```

## Docker
```bash
docker build -t fastapi-app ./app
docker run -p 8000:8000 fastapi-app
```

## Kubernetes
```bash
kubectl apply -f k8s/
```
