# Session 4: A Closer Look at Canary Deployments

Homework for this session consists of reading a classic document on canary deployments and working through (or at least reading through) labs on implementing canary deployments with Google Cloud Platform (GCP) and Blue-Green deployments with Amazon Elastic Container Service (ECS).

## Why "Canary"?

The term "canary deployment" originated from the historical practice of using canaries in coal mines.

<p align="center">
  <img src="https://raw.githubusercontent.com/cicdsummerschool/session-4/main/images/canary-1.jpg" width=50% /><br>
  <ins><b><i>Miner in yellow helmet with canary in a cage.</i></b></ins>
</p>

Miners would carry canaries with them because these birds are more sensitive to toxic gasses like carbon monoxide. If the canary showed signs of distress or died, it was a warning to the miners that the environment was unsafe.

In software, a canary deployment involves releasing changes to a small subset of users first to detect any potential issues before rolling out to everyone.

<p align="center">
  <img src="https://raw.githubusercontent.com/cicdsummerschool/session-4/main/images/canary-2.jpg" width=50% /><br>
  <ins><b><i>Canary between two racks of super computers.</i></b></ins>
</p>

## [Canary Release by Danilo Santos, Thoughtworks](https://martinfowler.com/bliki/CanaryRelease.html)

The article explains the concept of a Canary Release, a strategy for minimizing risk when deploying new software versions. It involves gradually rolling out the update to a small subset of users before full deployment. This method allows for real-time monitoring and quick rollback if issues arise, making it a safer alternative to deploying across the entire infrastructure at once. The article also discusses strategies like using Phoenix or Immutable Servers and highlights challenges such as managing multiple software versions simultaneously.

- Full article [here](https://martinfowler.com/bliki/CanaryRelease.html).

## [Cloud Run Canary Deployments](https://www.cloudskillsboost.google/focuses/52827?parent=catalog)

- _**This lab is being shared as a reference only.  Browse through the steps to get an idea of the process.  Because of changes in the Google Cloud Service, this lab may not be able to be completed successfully (or without encountering lots of errors).**_

- _The content in this lab is associated with the Cloud Skills Boost service.  The lab is intended to be run using a Cloud Skills Boost account.  With that in mind, some of the instructions may not apply to the use of the lab outside of the intended environment._

- _If you encounter a prompt that indicates the lab content is not available, select **Yes, notify me**._

- _If you aren't able to access the content from the link above, a PDF copy of the lab is available here: [Cloud Run Canary Deployments PDF](./images/cloud-run-canary-deployments-google-cloud.pdf).  Note that some of the content in the PDF may be obscured.  Just browse through the document to get an idea of how a canary deployment is implemented using Google Cloud Run._

In this lab you will learn how to implement a deployment pipeline for Cloud Run that executes a progression of code from developer branches to production with automated canary testing and percentage based traffic management.


## [Blue/Green Deployments :: Amazon ECS Workshop](https://ecsworkshop.com/blue_green_deployments/)

The article from the Amazon ECS Workshop explains Blue/Green Deployments, a method for deploying applications by shifting traffic between two identical environments (Blue and Green) running different versions of the same application. This approach allows for validation of the new version (Green) while keeping the old version (Blue) live, ensuring minimal risk and easy rollback if issues arise. This technique is particularly useful for critical workloads where downtime or impaired operation must be minimized.

- Full article [here](https://ecsworkshop.com/blue_green_deployments/).

## [Deploying an Amazon ECS service using a blue/green deployment](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create-blue-green.html)

The AWS documentation provides a detailed guide on implementing Blue/Green Deployments using Amazon ECS and AWS CodeDeploy. It walks through setting up the necessary infrastructure, including load balancers, ECS clusters, and task definitions. The guide also covers the creation of deployment groups and CodeDeploy resources, and how to monitor and manage the deployment process. It ends with instructions on cleaning up resources to avoid unnecessary charges.

- Full article [here](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create-blue-green.html).

<!-- FooterStart -->
---
[← Session 3: Deployment Methods for Every Scale](../session-3/README.md) | [Session 5: CI/CD Security →](../session-5/README.md)
<!-- FooterEnd -->
