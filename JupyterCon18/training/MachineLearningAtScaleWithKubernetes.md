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

### lab 1 - https://qwiklabs.com/focuses/1029?parent=catalog - Introduction to Docker
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

### lab 2 - https://qwiklabs.com/focuses/564?parent=catalog - Hello Node Kubernetes

* https://www.youtube.com/watch?v=fRYEJmRMkQk&feature=youtu.be
* to connect to outside world must expose pod as a service

### GKE - google kubernetes engine
* googel managed kubernetes master
* work nodes
* master uptime - 99.5% managed by google project ( you manage the nodes project)

### lab 3 - https://qwiklabs.com/focuses/557?parent=catalog - Orchestrating the Cloud with Kubernetes
* Provision a complete Kubernetes cluster using Kubernetes Engine.
* Deploy and manage Docker containers using kubectl.
* Break an application into microservices using Kubernetes' Deployments and Services.
* https://cloud.google.com/sdk/gcloud/

## afternoon

### running tensorflow on kubernetes --> kubeflow (launch 2/2018)
* https://github.com/kubeflow/kubeflow
* composable, portable, scalable
* before tensor processing unit (TPU), it ws jelly doughnut and jellyfish
* kubeflow
  * jupyter notebook (or hub)
  * multi-architecture, distributed training
  * model serving
  * ??
  * ??
  * trainer,build model,model validation,training at scale, serving
* tech --> finance --> regular dudes
* open
* components
  * bootstrap container
  * ambassador service
  * cloud identity aware proxy
  * jupyter service and hub
  * tensorflow transform - library for preporcessing data with tensorflow
  * TFMA - tensorflow model analysis (library)
  * TF Job - custom resource, easy to run distributed or non- distributed TensorFlow jobs
  * Argo CD uses GitOps pattern
  * Seldon , 
  
### lab 4 - https://qwiklabs.com/focuses/960?parent=catalog - Introduction to Kubeflow on Google Kubernetes Engine

### lab 5 - https://google.qwiklabs.com/focuses/1257?locale=en&parent=catalog - kubeflow end to end lab
