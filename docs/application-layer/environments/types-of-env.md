# Types of Environments

### Production Environment

This is the default environment for your project where your final and polished app should reside. A `Production` environment can only have its own dedicated resources and cannot be shared with any other environment to maintain the highest level of performance,security and reliability.

!!! warning "Warning"

    `Production` cannot be deleted or created. It is generated automatically upon project creation and can only be removed when the same project is deleted. You can only update and scale the Production environment.

### Staging Environment

This environment is to test your application before sending the application to production. Just like the `Production` environment, it also has dedicated resources by default and are not shareable with others, ensuring privacy during testing and development.

### Development Environment

The `Development` environment is the stage for experimenting and trying out new features. You can have either dedicated resources or share it with any other dedicated environment.

### Custom Environments

The `Custom` environment is versatile and fully customizable to the liking of user. Unlike the other environments, you can create as many `Custom` environments as you want. You also have the option to share the resources of this environment with other dedicated environments or keep it dedicated, depending on your specific needs.
