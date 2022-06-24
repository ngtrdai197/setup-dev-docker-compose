.PHONY: up

up:
	@echo "Up mysql db ... "
	docker-compose up

.PHONY: build
build:
	@echo "Building mysql db ..."
	docker-compose up --build

.PHONY: upd
upd:
	@echo "Building mysql db and detach ..."
	docker-compose up --build -d

.PHONY: down
down:
	@echo "Downing mysql db ..."
	docker-compose down

.PHONY: downvl
downvl:
	@echo "Downing and remove volume mysql db ..."
	docker-compose down -v
