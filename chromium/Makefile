IMAGE_NAME=joinsolutions/chromium
CHROMIUM_VERSION=101.0.4951.54

docker:
	docker build --pull -t $(IMAGE_NAME):$(CHROMIUM_VERSION) .

push:
	docker push $(IMAGE_NAME):$(CHROMIUM_VERSION)
