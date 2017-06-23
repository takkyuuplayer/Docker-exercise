DOCKER=$(shell which docker)
DOCKER_COMPOSE=$(shell which docker-compose)
CONTAINER_NAME=nginx_test

up:
	$(DOCKER_COMPOSE) up -d

build:
	$(DOCKER_COMPOSE) build

clean:
	$(DOCKER_COMPOSE) stop
	$(DOCKER_COMPOSE) rm -f

attach:
	@$(DOCKER) exec -it $(CONTAINER_NAME) bash
