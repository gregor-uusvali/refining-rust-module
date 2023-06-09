## Context
CI/CD (continuous integration / continuous delivery) allows us to automate software deployment.

A Github Actions (GHA) runner is a small program running on your server that follows the instructions defined in a github actions workflow.

## Task
Setup a self-hosted Github Actions runner on your server and implement github actions workflow for your repository.

The github actions runner should be able connect to github hub.
The github actions workflow should define steps to checkout your repository, run tests on the code, compile and build the artifact and deploy the artifact on your server.


## References
[Creating self-hosted runner](https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/adding-self-hosted-runners)


[Creating workflow](https://docs.github.com/en/actions/quickstart)


[Actions checkout (Checking out your repository)](https://github.com/actions/checkout)


[Github actions marketplace](https://github.com/marketplace)

## Learning outcomes
After this module, you should be able to create your own self-hosted GHA runner, run GHA workflows on the runner and automate your application deployment via CI/CD