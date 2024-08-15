ELASTICSEARCH_VERSION = latest

NAMESPACE = default

DOCKER_IMAGE_NAME = my-elastic-image
DOCKER_IMAGE_TAG = $(ELASTICSEARCH_VERSION)

K8S_DEPLOYMENT_NAME = elasticsearch
K8S_SERVICE_NAME = elasticsearch

build-docker-image:
	docker build -t $(DOCKER_IMAGE_NAME):$(DOCKER_IMAGE_TAG) .

push-docker-image:
	docker push $(DOCKER_IMAGE_NAME):$(DOCKER_IMAGE_TAG)

shell:
	kubectl exec -it deployment/$(K8S_DEPLOYMENT_NAME) /bin/bash

logs:
	kubectl logs -f deployment/$(K8S_DEPLOYMENT_NAME)
	