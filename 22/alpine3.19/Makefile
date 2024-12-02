# Makefile for building multi-platform Docker images

PLATFORMS := linux/amd64,linux/arm64
IMAGE_NAME := node:22.11.0-alpine3.19

build:
	docker buildx build --platform $(PLATFORMS) -t $(IMAGE_NAME):latest .

push:
	docker buildx build --platform $(PLATFORMS) -t $(IMAGE_NAME):latest --push .

