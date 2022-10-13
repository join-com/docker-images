IMAGE_NAME=joinsolutions/cimg-node
IMAGE_VERSION=14.20.1-browsers

docker:
	docker build --pull -t $(IMAGE_NAME):$(IMAGE_VERSION) .

push:
	docker push $(IMAGE_NAME):$(IMAGE_VERSION)
