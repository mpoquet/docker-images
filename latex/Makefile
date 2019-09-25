default:
	@echo "Try make build, make build-nocache or make push."

build:
	docker build -t mpoquet/latex_ci:latest \
                 -t mpoquet/latex_ci:$$(date --iso-8601) \
                 .

build-nocache:
	docker build -t mpoquet/latex_ci:latest \
                 -t mpoquet/latex_ci:$$(date --iso-8601) \
                 --no-cache \
                 .

push:
	docker push mpoquet/latex_ci
