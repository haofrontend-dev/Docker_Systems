include .env
export $(shell sed 's/=.*//' .env)

# Folder contants
DOCKER_COMPOSE_DEV := docker-compose.dev.yml
DOCKER_COMPOSE_PROD := docker-compose.prod.yml

# Run auto
default:
	docker ps

############# Dev #############
run-build-dev:
	docker-compose -f $(DOCKER_COMPOSE_DEV) up -d --build


run-down-dev:
	docker-compose -f $(DOCKER_COMPOSE_DEV) down

############# Prod #############
run-build-prod:
	docker-compose -f $(DOCKER_COMPOSE_PROD) up -d --build
	
run-down-prod:
	docker-compose -f $(DOCKER_COMPOSE_PROD) down	