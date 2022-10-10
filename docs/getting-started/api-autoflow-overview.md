---
layout: default
title: API AutoFlow Overview
parent: Getting Started
nav_order: 1
---
# Getting started: It's all about the solution.

**You don't have to be proficient at coding. If you know the concept of `IF` conditions and `Loop` iteration, that all you need.**

Welcome to API AutoFlow!

Whether you're building your own social network, opening an eCommerce site, integrating APIs, or managing a company's API infrastructure, API AutoFlow helps you create and integrate anything you can imagine to create the solution that matters to you. You decide what your [solution](#whats-a-solution) has to do by build the perfect data and automation [flows](#whats-a-flow) for your needs.

Unlike traditional no-code platforms that are made for the `frontend`, API AutoFlow gives you the power of a super-flexible `backend` to connect your services and design the perfect data [flows](#whats-a-flow) all in one place.

## Main points
* A [solution](#whats-a-solution) is a collection of flows and related components.
* A [flow](#whats-a-flow) is a dataflow that passes data from one action to another to achieve the intended result. A flow takes an input data, takes actions on the data, and outputs the resulting data.

{% include in_line_banner.html url="../../tutorial-video" title="Quick Start with Free Training Videos" button_name="Watch a training" message="! Get started faster with API AutoFlow" %}

When you first open up API AutoFlow, you'll see a bunch of colorful icons arranged into different groups. The groups are solutions, and the icons are flows.



# It's all about APIs


## Overall Application Architecture?
API AutoFlow is the **application backend** that processes the data and performs automation logic.

![Application Architecture](/assets/images/getting-started-index-application-architecture.jpg)
_API AutoFlow is one of the few no-code platform available for backend_

* **Frontend**: Client-side including Angular, React, Vue, Xcode, Flutter, sensors, robots, devices, etc
* **Backend**: Server-side including **API AutoFlow**, JAVA, PHP, Javascript, Node, Python, Laravel, Django, C, Ruby, etc
* **Data Source**: Including databases, APIs, other applications, sensors, robots, devices, etc

Now you know what API AutoFlow can do, but you still might not know where to begin so let's start with what you first see when you sign in to API AutoFlow.

## What's a solution?
A solution is a collection of flows and related components. The founder of a startup business might want to build a quick MVP solution for investor pitch or customer feedback; an employee within a larger company might have its own solution that needs to integrate with customer legacy systems; a DevOps or operation team might have an automation built for collecting data and management the infrastructure.

When you open up your API AutoFlow homepage, you can see all the flows for which you're a collaborator.

![What's a solution](/assets/images/getting-started-index-solution.png)
_An example API AutoFlow homepage, with several flows organized into custom solutions._


For more information visit [solution]({% link docs/overview/definitions/solutions.md %}) details page


## What's a flow?
Each of the horizontal line in a solution represents a flow. A flow—that's short for "dataflow"-passes data from one action to another to achieve the intended result. A flow takes an input data, takes actions on the data, and outputs the resulting data. A flow can be a data transformation ETL/ELT pipeline, an process automation, your product's integration addon, an entire application backend, or really, anything you can imagine!

![What's a flow?](/assets/images/getting-started-index-flow.png)

Colorful boxes at the front of each flow are the endponints. Each of these endpoints represents the start of dataflow! You can make as many of them as you want.

For more information visit [flow]({% link docs/overview/definitions/flows.md %}) details page

## How to make a solution
The best way to understand what a solution does and how to use it is to go ahead and make one. There are a few different ways to create a new solution. Which option you choose will depend on how much you're looking for inspiration and guidance versus how much you already know about what you want your solution to do.

* **Templates**: If you're just getting started, API AutoFlow's [templates](#use-an-api-autoflow-template) demonstrate example solutions while serving as good starting points for building your own custom flow.
* **Marketplace**: If you're interested in discovering more about how real people use API AutoFlow, try making a copy of a flow from API AutoFlow [marketplace](#explore-api-autoflow-marketplace).
* **Shared Configurations**: If you're coming from a team that's already using API AutoFlow, you can take your team's API AutoFlow [configuration](#import-a-configuration-file-and-turn-it-into-a-solution) file and turn it into your solution.
* **From Scratch**: If you know what you're doing (or if you're following this guide!), you can create a solution from [scratch](#build-a-flow-from-scratch) to your exact specifications.

No matter which option you choose, you can always customize your solution's flow and data later—so don't stress out too much about which option you pick.

### Use an API AutoFlow template

<!-- <div>
  <a href="" style="width: 200px; height: 150px; border: 1px solid grey; margin: 2px; padding: 2px 5px; display: inline-block; text-align">
    <div style="height: 100%; width: 30px; display: inline-block; vertical-align: top">
      <img src="/assets/images/getting-started-index-solution.png" style="width:25px"/>
    </div>
    <div style="height: 100%; display: inline-block; color: grey">
      <div style="font-size:1.3em; font-weight: 500">To Do App</div>
      <div>asdf</div>
      <div><span>no-code</span></div>
    </div>
  </a>
  <a href="" style="width: 200px; height: 150px; border: 1px solid grey; margin: 2px; padding: 2px 5px; display: inline-block; text-align">
    <div style="height: 100%; width: 30px; display: inline-block; vertical-align: top">
      <img src="/assets/images/getting-started-index-solution.png" style="width:25px"/>
    </div>
    <div style="height: 100%; display: inline-block; color: grey">
      <div style="font-size:1.3em; font-weight: 500">To Do App</div>
      <div>asdf</div>
      <div><span>no-code</span></div>
    </div>
  </a>
</div> -->

The team here at Interactor are continuously making templates designed for specific use cases, like an CRM, a social media, a eCommerce, or a chatbot such as Slack replica. These templates are solutions that come pre-configured with the full stack scalable architecture including the `frontend`, `backend`, and `database / data source`. If you're still learning the API AutoFlow ropes, check out a template or two for inspiration—you can always modify it later to suit your own needs!

{% include in_line_banner.html url="https://www.interactor.com/product/autoflow/solutions/templates" button_name="Get Templates" message="! Get started faster with API AutoFlow Templates" %}

There are several ways to use a template:

* :cloud: **Cloud**: The templates are listed on popular cloud markplaces including AWS, Azure, Google, IBM, and Oracle
* :whale: **Docker**: The docker image with the entire application can be loaded using the `path` provided in the template
* :arrow_down: **On-premise**: The template provides the complete application including `frontend` code, `backend` API AutoFlow configuration, and `database` schema.  However, to run it [on-premise](#running-your-own-api-autoflow), you'll need to set up the environment including database and API AutoFlow installation.

![Use an API AutoFlow template](/assets/images/getting-started-index-template.png)

If you want more information on any of the templates, click on its card and you'll go to that template's page—from here, you can read a more detailed guide on that flow and try a demo version of the template. Once you find a template you like, follow the instructions to instantiate on the cloud or download the template to make your very own copy!

Templates come with example records to make it easier to understand how they're set up. Once you've made your copy, you can delete those records whenever you want and instead fill in the template with your own information.

<!-- ### Explore API AutoFlow Marketplace
API AutoFlow enthusiasts from all over have made their own solutions, flows, and decided to share those flows with the rest of the world by publishing them on API AutoFlow Marketplace! Try browsing through API AutoFlow Marketplace for ideas and if you're feeling inspired, you make a copy of any solution on API AutoFlow Marketplace and customize it for your own needs.

To get to API AutoFlow Marketplace, click on the Marketplace at the top of the Interactor.com website or search for Github repository with the topic **apiautoflow** [https://github.com/topics/apiautoflow](https://github.com/topics/apiautoflow).

![Explore API AutoFlow Marketplace](/assets/images/getting-started-index-marketplace.png)

From the Marketplace page, you can type in search terms or left pane sort to look for relevant flows or click through the different categories on the side.

To find out more about a flow, go ahead and click on one of the flow cards. This will bring you to that flow's guide page, where the creator can explain the story behind the flow and how to use it.

If someone's made a flow that you want to make a copy of, click the clone flow button to make your very own copy! (And maybe give the creator a ❤️ on their flow, if you're feeling so inclined.)

Marketplace flows might or might not come prefilled with information. Once you've made your copy, you can delete any preexisting content whenever you want and instead fill in the template with your own information. And perhaps one day—maybe after finishing this guide—you'll be the one publishing your flows on API AutoFlow Marketplace for other users to copy on the Github. -->

## Running API AutoFlow
There are two way to access API AutoFlow

* **SaaS (*Beta*)**: Limited functionality.  Go to [https://console.apiautoflow.com](https://console.apiautoflow.com) and register using your email
* **On-premise**: Download a trial version by going to [https://www.interactor.com/product/autoflow/download](https://www.interactor.com/product/autoflow/download)

Once you get the access to API Autoflow you can either `upload` the solution or create from `scratch`

### Upload a configuration file and turn it into a solution
If you're coming from a team that already uses API AutoFlow, you can take the team's configuration file and turn it into your own solution. To upload the configuration file, go ahead and click the `Upload Configuration` button. This will open up a pop-up. Here, you can select the `config.json` file from your computer.

![Import a configuration file and turn it into a solution](/assets/images/getting-started-index-config.png)

This will bring up a dialog in which you can upload your configuration. Alternatively, if only a part of the flow is shared, you can also paste the configuration using the paste icon.

Note you can import part of the configuration and import more flows from other configurations later.

![Select flow to upload from the configuration ](/assets/images/getting-started-index-config-upload-select.png)

### Build a solution from scratch
Lastly (but certainly not leastly), you can always create a solution from scratch. If you're starting from scratch, it helps to know a little bit about how you're planning to structure your solution—but no matter what, you can always change your solution later, so feel free to build a solution from scratch even if you don't yet know what you're making.

![Build a flow from scratch](/assets/images/getting-started-index-scratch.png)

To make a solution from scratch, follow the training videos by pressing the link below or going to the `Training - Video` section on the left navigation.

{% include in_line_banner.html url="../../tutorial-video" title="Quick Start with Free Training Videos" button_name="Watch a training" message="! Get started faster with API AutoFlow" %}

{: .fs-6 .fw-300 }