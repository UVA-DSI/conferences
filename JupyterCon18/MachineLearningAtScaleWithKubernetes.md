## "Five Labs and Bunch of Slides"
* containers,kubernetes, google kubernetes engine, kubeflow, ksonnet, tensor2tensor

### setup
* use qwiklab credits, and GCP test accounts
* Kubernetes in qwiklabs: https://qwiklabs.com/quests/29

### containers
* what containers, what dockeer, why docker
  * Dedicated: Application, Dependences, Kernel, Hardware
  * VM: {Application, Dependences, Kernel}, Hardwarek
  * Container: {Application, Dependencies}, Kernel+Container Runtime, Hardware
* faster deployment, portable
* Docker
  * container
  * runtime
  * today: runtime, builds runs monitors containers
  * cgroups, namespaces - controls what containers seeq

### lab 1
* https://docs.docker.com/engine/reference/builder/#known-issues-run
* gcr: google container registry
* Ran containers based on public images from Docker Hub.
* Built your own container images and pushed them to Google Container Registry.
* Learned ways to debug running containers.
* Ran containers based on images pulled from Google Container Registry.

### kubernetes
* "kuberentes is two things to me: abstraction over infrastructure and set of declarative APIs."
  * tell what you need not what to do and let kubernetes figure out what to do
* built by googlers in 2014, goes by K8s
* master and worker nodes: each is a vm
* worker nodes are livestock not pets
* The Pod
  * the atom
  * one or more containers with shared networking and storage
* Deployment - long running jobs (like a web site)
* Drop (run one time) - chron job
* Services - stable endpoint for pods
* Namespaces - 
* kubectl - commands you use the most, cli

### lab 2
* https://www.youtube.com/watch?v=fRYEJmRMkQk&feature=youtu.be
* to connect to outside world must expose pod as a service
