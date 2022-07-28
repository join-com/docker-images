IMAGE_NAME=joinsolutions/chromium
CHROMIUM_VERSION=103.0.5060.134

docker:
	docker build --pull -t $(IMAGE_NAME):$(CHROMIUM_VERSION) .

push:
	docker push $(IMAGE_NAME):$(CHROMIUM_VERSION)
