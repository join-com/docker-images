IMAGE_NAME=joinsolutions/chromium
CHROMIUM_VERSION=99.0.4844.84

docker:
	docker build --pull -t $(IMAGE_NAME):$(CHROMIUM_VERSION) .

push:
	docker push $(IMAGE_NAME):$(CHROMIUM_VERSION)
