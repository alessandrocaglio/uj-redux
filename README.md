# Ubiquitous Journey

This repo embodies a GitOps approach to deploying application code, middleware infrastructure and supporting CI/CD tools. 

At its simplest, the repo is an [ArgoCD Application](https://argo-cd.readthedocs.io/en/stable/core_concepts/) which references [other helm charts](https://github.com/redhat-cop/helm-charts.git) and [other kustomize definitions](https://github.com/rht-labs/refactored-adventure) to deploy applications.

The idea is to reference other Charts, Kustomize, YAML snippets from within this framework. This keeps things `pluggable` to suit the needs of your team.

We have evolved the design from the original [Labs CI / CD](https://github.com/rht-labs/labs-ci-cd.git) project. The  Ubiquitous Journey (`UJ`) represents a major milestone in moving to a GitOps approach to tooling, application management and configuration drift using [ArgoCD](https://argoproj.github.io/argo-cd/).

## Components

There are two main components to this repository:

1. `Ubiquitous Journey` - Contains all the tools, collaboration software and day2ops to be deployed on Red Hat OpenShift. This includes chat applications, task management apps and tools to support CI/CD workflows and testing. For the complete list and details: [What's in the box?](docs/whats-in-the-box.md)
2. An demo application called [`pet-battle`](https://github.com/petbattle) that shows you how to use the UJ structure with a three tiered application stack.

Each part can be used independently of each other but sequentially they create a full stack.