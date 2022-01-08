
.DEFAULT_GOAL := help
.PHONY: test 

help:
	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST)  | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'

test: ## Run tests 
	echo "Not implemented"

install-nvidia-docker: ## Install the dependency of the nvidia-docker
	chmod u+x ./scripts/install-nvidia-docker-dependency.sh 
	./scripts/install-nvidia-docker-dependency.sh 

generate-onnx: ## Generate onnx format 
	echo "Not implemented"

lint: ## Executing linting 
	echo "Not implemented"