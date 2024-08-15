# To deploy YAML files

deploy:
	kubectl apply -f kube-logging.yaml
	kubectl apply -f efk-ingress.yaml
	kubectl apply -f elasticsearch_svc.yaml
	kubectl apply -f kibana-service.yaml
	kubectl apply -f kibana-deployment.yaml
	kubectl apply -f fluentd.yaml
	kubectl apply -f elasticsearch_statefulset.yaml
	kubectl apply -f storage_class.yaml
	kubectl apply -f pv-definition.yaml

stop:
	kubectl delete -f kube-logging.yaml