NAME := bellx2/rasbian:jessie-dev

image:
	docker build --build-arg DEBIAN_FRONTEND=noninteractive -t $(NAME) .

push:
	docker push $(NAME)
