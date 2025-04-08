Cloud Migration Strategy comparison with Kubernetes

This project compares two cloud migration strategies using a lift app and cloud native application, containerizing them and then deploying them to Google Kubernetes Engine using the Google Cloud Platform

I evaluated them both strategies based on performance, cost efficiency and resource utilization. 

Project Overview
- Lift-and-Shift App: Traditional monolithic Flask app containerized and deployed without rearchitecting.
- Cloud-Native App: Modularized frontend + backend Flask apps built with microservice principles and deployed separately.
- Infrastructure: GKE (Autopilot mode), Kubernetes manifests, Dockerized apps.
- Testing: Locust used to simulate user traffic and generate load for analysis.

Folder Structure
-cloud-native-backend
  -app.py
  -backend-deployment.yaml
  -backend-service.yaml
  -Dockerfile
  -requirements.txt
-cloud-native-frontend
  -Dockerfile
  -frontend-deployment.yaml
  -frontend-service.yaml
  -index.html 
-lift-shift
  -flask-liftshift.yaml
  -flask-service.yaml
-test-loading
  -locustfile.py
-t-test.py

