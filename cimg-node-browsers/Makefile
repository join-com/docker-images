IMAGE_NAME=joinsolutions/cimg-node
IMAGE_VERSION=18.16.0-browsers

docker:
	docker build --pull -t $(IMAGE_NAME):$(IMAGE_VERSION) .

push:
	docker push $(IMAGE_NAME):$(IMAGE_VERSION)
