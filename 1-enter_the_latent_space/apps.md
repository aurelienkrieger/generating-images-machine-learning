# End-user Applications

This is the central piece of your creative workflow. They are often refered to as GUI (Graphical User Interface) because they offer a graphical interface for you to load and train models, adjust parameters, run diffusion scripts etc. New models and GUIs are constantly being developed by the AI community, being individual developers, open source communities, academics or companies, so it is rapidly changing but we can identify 2 types of applications:

1. Local applications
  - manual installation
  - downloadable
  - containers
2. Online services
  - demos
  - cloud GPU services
  - integrated online platforms

## Local applications

Local applications are generally free and open source. If you have a compatible hardware, you can install them locally on your computer to generate images. Some have downloadable binary files, other require more technical knowledge to install all the dependencies. There are also containers, like the platform Docker, which is a way to deliver software in packages so you don't have to install everything manually.

## Online services

If your GPU is not powerful enough or you have issues going through the process of setting up the GUI manually, you can use online services. The common idea of these services is to make GPUs available on the cloud through a web interface, so you don't run the scripts on your computer but rather make requests from a website. Some are free demos, just to test a model. Others are cloud services where you have to manually install a script or application to generate images, they offer more flexibility but require more technical knowledge. Finally you have fully-integrated commercial platforms that aim to streamline the process of setting up a GUI and generating images.

## Best options _(at the moment)_

The criteria used to select the GUI used in this course are:

1. Open Source
  - as the technology is rapidly evolving, open source licensing is the best way to allow the whole community to use, investigate and improve the systems
  - it is also the best option to run the applications for free on a compatible hardware, without being tracked or liable to monthly plans
2. Good balance between functionality and accesibility
  - some GUI are extremely powerful because they are open system where anyone can develop extensions, but can be harder to use
  - considering the concepts remain the same, the course focuses on easy to install / easy to use GUI that can still offer a good level of flexibility

According to these standards, the best 3 GUI at the moment seem to be:
- AUTOMATIC1111 is very powerful because it allows a lot of customization but it can get overwelming
- ComfyUI is considered the fastest of all, but its interfaces uses graphical nodes, which is not necessarily accesible for everyone
- InvokeAI, seem to offer a good balance. Its interface is built around a graphical canvas that is more intuitive for creative profesionals. It is accessible for free locally, but the company also offers an online service to run the GUI on their servers.

Note: [RunDiffusion](https://rundiffusion.com/) is a cloud service that offers fully managed Open Source GUIs like AUTOMATIC1111, ComfyUI and InvokeAI.

## Resources

[Useful links & tutorials about End-User Applications](../resources/apps.md)
