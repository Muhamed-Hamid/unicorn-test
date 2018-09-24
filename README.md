# unicorn-test

This is a dockerized ruby app.

1# Create an image for this app
$ docker build -t drkiq .

2# We create our resources for Kubernetes
we need to make our configmap, it's created as mymap.

$ cd kube/ruby/ && kubectl create -f services.yml && kubectl create -f secret.yml\
	kubectl create -f drkiq-Vol.yml && kubectl create -f postgres-Vol.yml \
	kubectl create -f redis-vol.yml
	kubectl create -f deply.yml
