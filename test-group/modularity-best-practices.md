---
description: >-
  this page contains the first draft of the modularity best practices - it
  teaches HOW to create modularity, not WHY/WHEN
---

# Modularity \(best practices\)

### Reusable elements

Reusable elements are a Bubble tool that allow us to create an element once and use it in several places throughout an application. When we make a change to this element, that change is immediately made in all the places that the element appears throughout the app.

Bubble's default apps also use reusable elements - they come with a header, footer, and a signup/login popup.

### Custom Workflows

**Custom workflow**: a workflow that can be triggered from other workflows and that accept one input.

The custom workflow below can be triggered anywhere from this reusable element, and can also be triggered from any page or reusable element that contains the signup/login reusable element.

This workflow doesn't have any inputs passed through it, as seen by the empty **Type of thing** dropdown.

The above custom workflow is admittedly complex, and displays several ways of making application logic modular. 

1. This is a **custom workflow** which then **triggers another custom workflow**. Logic in custom workflows can be easily changed, which is then reflected anywhere that the workflow is triggered.
2. This custom workflow calls an **API Workflow**, which moves some logic to a workflow that is run in the cloud \(not on your user's browser\). As a result, the logic is accessible from anywhere throughout the application. 
3. Note that this workflow is found inside the `signup/login` **reusable element**, so that it can easily be triggered from any page in the app where this reusable element is present.

### API Workflows

**API Workflow**: a workflow that is run somewhere in the cloud instead of on your user's browser. These workflows can be run \(nearly\) immediately or scheduled for a specific date and time in the future. API Workflows can take any number of inputs, and the inputs can be of any type.



{% hint style="info" %}
Note the various API workflows that are scheduled from the create\_email\_verification workflow. Building modularly allows us to create workflows that are both more complex, but still flexible and relatively easy to change.
{% endhint %}

### Plugins

**Bubble plugins** allow you to share functionality across multiple Bubble applications, giving plugins a special kind of cross-Bubble modularity.

Plugins are like tiny programs that do one or a couple small tasks. For example, plugins can be used to standardize the way you set up in-app notifications using the[ AirAlert plugin](https://bubble.io/plugin/airalert-1515787032525x876315403042684900). Or, you could set up a [Rich Text Editor](https://bubble.io/plugin/trix-rich-text-editor-1521223759938x925805827977117700) that allows users to compose text in an environment that is more similar to a word processor than a text box.

### App Templates

**App Templates** are a more unique and labor-intensive way of working modularly, and are more relevant to Bubble developers who will build many apps. This is what our [AirDev Canvas template]() is meant to do - it makes it so that builders can more quickly make fully-featured applications, without having to waste time on setup that you will do with every app you create.

### AirDev Canvas

**AirDev Canvas** allows you to build apps more quickly in a way that creates a visually consistent user experience across mobile and desktop. You can add modules that we have designed and build functionality on top of them, making it a breeze to create pages that look and work great.

