all: push

TAG = 2.7.002
PREFIX = k8s-registry.zeusis.com:32000/hadoop

container:
	docker build -t $(PREFIX):$(TAG) .

push: container
	docker push $(PREFIX):$(TAG)

clean:
	docker rmi $(PREFIX):$(TAG)
