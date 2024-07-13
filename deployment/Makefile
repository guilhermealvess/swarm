create-network:
	docker network create --driver overlay nginx_network

deploy-portainer:
	docker stack deploy -c portainer-agent-stack.yml portainer

deploy-api:
	docker stack deploy -c api-stack.yml api

deploy-nginx:
	docker stack deploy -c nginx-stack.yml nginx

deploy: create-network deploy-portainer deploy-api deploy-nginx