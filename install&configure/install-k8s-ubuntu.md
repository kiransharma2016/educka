
## Install K8s:  ubuntu 18 LTS WITH 2 CPUS & 4GB RAM
```
	sudo apt-get update
	sudo apt-get install -y apt-transport-https ca-certificates curl software-properties-common

	curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
	sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
	sudo apt-get update ; clear
	sudo apt-get install -y docker-ce
	sudo service docker start ; clear

	echo "deb http://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee /etc/apt/sources.list.d/kubernetes.list
	curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
	sudo apt-get update ; clear
	sudo apt-get install -y kubelet kubeadm kubectl
```
