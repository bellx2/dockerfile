NAME := bellx2/rasbian-x86_64:bullseye-dev

image:
	docker build -t $(NAME) .

run:
	docker run -it $(NAME)

push:
	docker push $(NAME)

clean:
	docker rmi -f $(NAME)