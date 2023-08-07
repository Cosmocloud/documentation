# Creating Environments

In our application, we have a feature called `Environments` that allows you to organize your work and collaborate efficiently. You start with a default `Production` environment, and you can create more environments to suit your needs! Let's see what each environment offers:

### Production Environment

This is the main stage for your project where your final and polished app resides.It has dedicated resources and cannot be shared with any other environment to maintain the highest level of performance,security and reliability.

!!! warning "Warning"

    `Production` cannot be deleted or created. It is automatically created and deleted with the project itself. You can only update and scale the Production environment

### Staging Environment

This environment is to test your application before sending the application to production. Just like the `Production` environment, it also has dedicated resources by default and are not shareable with others, ensuring privacy during testing and development.

### Development Environment

The `Development` environment is the stage for experimenting and trying out new features. You can share this environment with your team, making it easy to collaborate and work together. It also provide feature to share resources with other environments depending on your specific needs.

### Custom Environment

The `Custom` environment is versatile and fully customizable to the liking of user. Unlike the other environments, you can create as many `Custom` environments as you want. You also have the option to share this environment with others or keep it dedicated, depending on your specific needs.

# How to Create an Environment

1. Click on the `Create Environment` button in the Environments section.
2. Choose the type of environment you want to create: `Staging`, `Development`, or `Custom`.
3. If you select `Custom,` you can give it a unique name and set its sharing options.
4. For `Production` and `Staging,` the resources are automatically set to `Dedicated` for optimal performance.
5. For `Development` and `Custom,` you can specify whether you want dedicated resources or sharing with other environments.

<iframe src="https://drive.google.com/file/d/10LUdcScgiWxfgmC9zmDblt-2VOB2DNBv/preview" width="720" height="410" allow="autoplay"></iframe>

!!! info "Info"

    `Production`,`Staging` and `Development` environments can only be created once. For creating multiple environmets select `Custom` environment instead.
