# Types of Environments

### Production Environment

This is the default environment for your project where your final and polished app should reside. A `Production` environment can only have its own dedicated resources and cannot be shared with any other environment to maintain the highest level of performance,security and reliability to your application.

!!! warning "Warning"

    `Production` environment cannot be created or deleted manually. It is created automatically on project creation and can be removed when the project gets deleted. You can only update the tier of the Production environment.

### Staging Environment

The `Staging` environment is to test your application before deploying the application to production. This environment deployments are mainly used by testers to test the application end to end and find bugs.Like the `Production` environment, it also has dedicated resources.

### Development Environment

The `Development` environment is to create the APIs, Models and experimenting with other features that will not cause any issue in `Staging` or `Production` deployments. It can have dedicated resources or shared resources with any other dedicated environment.

### Custom Environments

The `Custom` environment is a customized environment which can be used by different teams to develop or test specific features and like, `Development` environment it can have either dedicated or shared resources based on the requirement of the user and unlike other environment types, there can be multiple custom environments.