# Continuous Deployment

Continuous Integration, Delivery, and Deployment are important devOps practices and we often hear a lot about them. These processes are valuable and ensures that the software is up to date timely.

- **Continuous Integration** is an automation process which allows developers to integrate their work into a repository. When a developer pushes his work into the source code repository, it ensures that the software continues to work properly. It helps to enable collaborative development across the teams and also helps to identify the integration bugs sooner.
- **Continuous Delivery** comes after Continuous Integration. It prepares the code for release. It automates the steps that are needed to deploy a build.
- **Continuous Deployment** is the final step which succeeds Continuous Delivery. It automatically deploys the code whenever a code change is done. Entire process of deployment is automated.

## What is GitOps?
GitOps in short is a set of practices to use Git pull requests to manage infrastructure and application configurations. Git repository in GitOps is considered the only source of truth and contains the entire state of the system so that the trail of changes to the system state are visible and auditable.

- Traceability of changes in GitOps is no novelty in itself as this approach is almost universally employed for the application source code. However GitOps advocates applying the same principles (reviews, pull requests, tagging, etc) to infrastructure and application
configuration so that teams can benefit from the same assurance as they do for the application source code.
- Although there is no precise definition or agreed upon set of rules, the following principles are an approximation of what constitutes a GitOps practice:
  - Declarative description of the system is stored in Git (configs, monitoring, etc)
  - Changes to the state are made via pull requests
  - Git push reconciled with the state of the running system with the state in the Git repository

## ArgoCD Overview
## Presentations

[GitOps Overview :fontawesome-regular-file-pdf:](../materials/05-Understanding-GitOps.pdf){ .md-button target=_blank}

## Activities

These activities give you a chance to walkthrough building CD pipelines using ArgoCD.

These tasks assume that you have:
 - Reviewed the Continuous Deployment concept page.

| Task                            | Description         | Link        | Time    |
| --------------------------------| ------------------  |:----------- |---------|
| ***Walkthroughs***                         |         |         |     |
| GitOps | Introduction to GitOps with OpenShift | [Learn OpenShift GitOps](https://docs.openshift.com/gitops/1.13/understanding_openshift_gitops/about-redhat-openshift-gitops.html){:target="_blank"} | 20 min |
| ***Try It Yourself***                         |         |         |     |
| ArgoCD Lab | Learn how to setup ArgoCD and Deploy Application | [ArgoCD](../../labs/devops/argocd/index.md) | 30 min |

Once you have completed these tasks, you will have created an ArgoCD deployment and have an understanding of Continuous Deployment.
