IMAGE_NAME=joinsolutions/chromium
CHROMIUM_VERSION=106.0.5249.91

docker:
	docker build --pull -t $(IMAGE_NAME):$(CHROMIUM_VERSION) .

push:
	docker push $(IMAGE_NAME):$(CHROMIUM_VERSION)
