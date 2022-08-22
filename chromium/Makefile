IMAGE_NAME=joinsolutions/chromium
CHROMIUM_VERSION=104.0.5112.101

docker:
	docker build --pull -t $(IMAGE_NAME):$(CHROMIUM_VERSION) .

push:
	docker push $(IMAGE_NAME):$(CHROMIUM_VERSION)
