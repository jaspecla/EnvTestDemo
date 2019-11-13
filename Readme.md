# Environment Deployment Demo for Azure Pipelines

This project is meant to show an Azure Pipelines CI/CD pipeline in YAML that supports deploying a web app to a dev environment and a prod environment.

Once your YAML pipeline is deploying to these environments, you can support manual approvals in the "Approvals and Checks" menu in your environment settings.
The documentation is somewhat confusing.  It indicates that only Kubernetes resources are supported in environments.  However, "resources" only indicates
the insights into the running Kubernetes environment. You can still run any tasks you like in the context of an environment, you just won't get the live-view experience
that you'd get with a "resource."

Note that you must have the multi-stage pipeline experience turned on in your Azure DevOps organization for this to work.