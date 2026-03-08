

DOCKER_USER        ?= chriswilling
mirror_base.x86_64 ?= http://192.168.1.16/slackware
mirror_base.i586   ?= http://192.168.1.16/slackware



x86_64:
	docker build -t $(DOCKER_USER)/slackware64-vmbuilder:current --build-arg mirror_base=$(mirror_base.x86_64) -f Dockerfile.x86_64 .

i586:
	docker build -t $(DOCKER_USER)/slackware-vmbuilder:current --build-arg mirror_base=$(mirror_base.i586) -f Dockerfile.i586 .
