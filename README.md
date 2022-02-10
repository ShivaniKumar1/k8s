# Intro to Kubernetes
-- Following steps are only for macOS -- 


# Prereqs
- docker from https://www.docker.com/get-started
- hypervisor: VirtualBox from https://www.virtualbox.org/

# Installing Kubernetes
- install kubectl: `curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/darwin/amd64/kubectl" `
- - documentation: https://kubernetes.io/docs/tasks/tools/install-kubectl-macos/
- make binary executable: `chmod +x ./kubectl`
- move file to `PATH`: `sudo mv ./kubectl /usr/local/bin/kubectl`
- test: `kubectl version --client`

# Installing minikube
- documentation: https://minikube.sigs.k8s.io/docs/start/
- installing: `curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-amd64`
- move to local bin: `sudo install minikube-darwin-amd64 /usr/local/bin/minikube`

# Verification
- docker: `docker version`
- minikube: `minikube version`

# Starting
- minikube: `minikube start`
- check if running: `kubectl get nodes`
