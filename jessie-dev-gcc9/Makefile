NAME := bellx2/rasbian-x86_64:jessie-dev-gcc9

image:
	docker build -t $(NAME) .

run:
	docker run -it $(NAME)

push:
	docker push $(NAME)

clean:
	docker rmi -f $(NAME)