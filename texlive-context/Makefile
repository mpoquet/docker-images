default:
	@echo "Try make build, make build-nocache or make push."

build:
	docker build -t mpoquet/texlive-context_ci:latest \
                 -t mpoquet/texlive-context_ci:$$(date --iso-8601) \
                 .

build-nocache:
	docker build -t mpoquet/texlive-context_ci:latest \
                 -t mpoquet/texlive-context_ci:$$(date --iso-8601) \
                 --no-cache \
                 .

push:
	docker push mpoquet/texlive-context_ci
