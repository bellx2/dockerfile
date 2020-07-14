NAME := bellx2/arm_ubuntu:xenial-dev

image:
	docker pull multiarch/ubuntu-core:x86_64-xenial
	docker build -t $(NAME) .

push:
	docker push $(NAME)

run:
	docker run -it $(NAME)

clean:
	docker rmi -f $(NAME)