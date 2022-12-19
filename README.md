# DevOps Take-home Assessment

## Instructions:
Fork this repo and follow the guidelines below. Try to spend 4 hours or less on the project. When finished or you've run out of time, link your forked repo back to Coterie for review.

## The Assignment:
As a DevOps Engineer at Coterie, you will be asked to create CI/CD pipelines for a variety of different solutions via GitHub Actions.  The most common solution you will need to deliver is a .NET API, containerized and deployed to a Kubernetes cluster.

In this repo there is a .NET 6 Solution which includes:
- a WebAPI Project
- a Contracts Project that should be packaged into a NuGet package 
- a Unit Test Project that should run and display passing tests

You should create two workflows:
- When a developer wants to make a change to the solution, they submit a PR from a working branch, which should trigger a build of the solution that runs unit tests
- When the PR is merged into the `main` branch a build is triggered, then is deployed to a development environment.  If the deployment to the development environment succeeds, it should automatically promote to the test environment. 

A Kubernetes cluster (or clusters) should be the target environments for the deployment.

## Requirements
- A build is triggered from a Pull Request
- A build and a deployment are trigged from a push to a `main` branch  
- A Dockerfile is created that containerizes the .NET WebAPI and is built
- A NuGet Package is output from the build (Publishing isn't required)
- Two Environments are configured.
- The .NET API is deployed to both environments

## That's a lot of moving parts...

There are **lots** of moving parts.  Between .NET API and NuGet builds, unit tests, docker builds, kubernetes deployments, and GitHub Actions workflows, there may be limitations on what you can accomplish in the recommended amount of time to complete this assessment.  100% Completion is encouraged, but **not required**.  

If you lack the necessary infrastructure to complete feel free to mock those (You can just use commented code if necessary), but feel free to spin up a trial account in Microsoft Azure (preferred) or another free provider if you want something fully featured.

## Questions
Feel free to reach out with questions or concerns regarding the assessment.  This is a free form assessment and is left vague to allow for multiple solutions to the project.
