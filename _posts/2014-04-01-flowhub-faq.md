---
layout: documentation
title: Flowhub FAQ
categories:
 - documentation
---

* [Popular Questions](#popular-questions)
  * [What is Flowhub?](#what-is-flowhub)
  * [Getting started](#getting-started)
  * [Example Apps](#example-apps)
  * [Browser Requirements](#browser-requirements)
  * [What runtimes/languages are supported?](#what-runtimeslanguages-are-supported)
  * [How about support for: insert favorite programming language.](#how-about-support-for-insert-favorite-programming-language)
  * [Does Flowhub require an internet connection?](#does-flowhub-require-an-internet-connection)
  * [It looks like this thing generates code.](#it-looks-like-this-thing-generates-code)
  * [Is this similar to UML?](#is-this-similar-to-uml)
  * [Sounds like a good idea, but drag and drop editors are crap, this thing brings back nightmares from BPEL or Yahoo!Pipes or: insert a 90's era flowchart looking thingy.](#sounds-like-a-good-idea-but-drag-and-drop-editors-are-crap-this-thing-brings-back-nightmares-from-bpel-or-yahoopipes-or-insert-a-90s-era-flowchart-looking-thingy)
  * [Where do I report bugs?](#where-do-i-report-bugs)
* [Privacy and Security](#privacy-and-security)
  * [Local Development Support](#local-development-support)
  * [Why does Flowhub need access to all public repos?](#why-does-flowhub-need-access-to-all-public-repos)
* [Payments/Licenses](#paymentslicenses)
  * [Pre-order License](#pre-order-license)
  * [Kickstarter License](#kickstarter-license)
  * [Lifetime Discount](#lifetime-discount)
  * [When will the pre-order period end?](#when-will-the-pre-order-period-end)
  * [What’s the current status of Flowhub?](#whats-the-current-status-of-flowhub)
  * [Where is the source code?](#where-is-the-source-code)

------------------------------------------------------------------------


## Popular Questions

###What is Flowhub?
Flowhub is a web-based IDE for flow-based programming. It is built on NoFlo.js for both client and server. It can connect to any language or environment that can talk the [FBP Network Protocol](http://noflojs.org/documentation/protocol/).

###Getting started
To get started with Flowhub, use the Flowhub getting started docs above. To get started with Flow-based Programming and NoFlo in general, Visit the [NoFlo Documentation](http://noflojs.org/documentation/).

###Example Apps
Client-side example: [Photobooth](http://flowhub.io/demo/photobooth/)  
Client-side example: [Clock](http://app.flowhub.io/#example/7135158)

###Browser Requirements
We recommend Chrome 33+ or Firefox 28+. Flowhub aims to support [evergreen browsers](http://www.yetihq.com/blog/evergreen-web-browser/). This means we support the most recent versions of Chrome, Safari, Internet Explorer, and Firefox.

###What runtimes/languages are supported?
* Client-side JavaScript for Browser (NoFlo)
* Server-side JavaScript for Node.js (NoFlo)
* Desktop programming for GNOME (NoFlo)
* Microcontrollers ([MicroFlo](https://github.com/microflo/microflo))
* Image processing ([ImgFlo/GEGL](https://github.com/imgflo/imgflo))
* Message queues ([MsgFlo]((https://github.com/msgflo/msgflo))

###How about support for: insert favorite programming language.
Flow-Based Programming is a paradigm that can be adapted to work with any existing programming languages. The user interface layer has been designed to be independent of the underlying FBP implementation, and so the various programming communities should be able to connect it with their flow-based environments. Making it work with Actor Based and Functional Reactive systems should be especially easy.

Please refer to the [FBP Network Protocol documentation](http://noflojs.org/documentation/protocol/) for details how to connect your own Flow-Based or dataflow environment with Flowhub.

###Does Flowhub require an internet connection?
No, Flowhub is built with the [offline first](http://offlinefirst.org/) philosophy, and works fine without an internet connection once you've installed it.

Some parts of Flowhub, like GitHub synchronization or real-time collaboration however require an internet connection to work. Access to runtimes may depend on connectivity depending where they are running.

###It looks like this thing generates code.
NoFlo does not generate code, but graphs can be exported as JSON.

###Is this similar to UML?
This is not a rehash of UML. UML is a diagram mapping out object-oriented constructs, often used for code generation. NoFlo graphs instead are only the coordination layer that manages the control flow of your software. The components are still handcrafted and unit-tested code that NoFlo merely wires together at runtime, following the edges specified in a JSON file. No code generation here.

###Sounds like a good idea, but drag and drop editors are crap, this thing brings back nightmares from BPEL or Yahoo!Pipes or: insert a 90's era flowchart looking thingy.
The story of visual programming tools started with the GRaIL system of the 60s, and has progressed to tools like LabView and Pure Data. So far none of these tools has reached mainstream acceptance outside of their (sometimes fanatic) industry niches. This is partly because these tools were built originally with a particular problem domain in mind, and partly because of the user experience. Execution matters, as we've seen so many times in the tech industry. After all, there were a lot of tablets before the iPads.

###Where do I report bugs?
If you find a bug, please report it on the [NoFlo-UI Github issue tracker](https://github.com/noflo/noflo-ui/issues).

## Privacy and Security

###Local Development Support
All source code for graphs and components is primarily stored locally inside your browser's [Indexed Database](http://en.wikipedia.org/wiki/Indexed_Database_API) storage, and only transmitted to GitHub when you choose to push your code.

When you wish to run the graphs on a flow-based runtime environment, for example on NoFlo running on Node.js, the Flowhub application talks with that runtime directly and your source code never passes through our servers. Flowhub's network services are used for runtime discovery, however.

The Flowhub application ships with a bundled NoFlo runtime for the browser. The [other runtimes](#what-runtimeslanguages-are-supported) can be run on your own machine(s) or deployed to some cloud service.

###Why does Flowhub need access to all public repos?
We need repository access to be able to push and pull the changes you make in Flowhub. Unfortunately GitHub's permission model only allows access to all public repositories, all public & private repositories, or no repositories at all. So to be able to provide GitHub integration we need this permission.

However, a possible workaround is to create a secondary GitHub user for Flowhub usage, and add that as a collaborator to the projects you want to work on in Flowhub.

## Payments/Licenses

###Pre-order License
Flowhub is free to use for public projects and open source development. Private project development & collaboration is reserved for paid plans. Pre-order licenses are offered during the pre-order period at a discount to regular pricing. Pre-order licenses will automatically convert to their respective higher priced paid plans upon public release of Flowhub.

You can view the different pre-order license tiers and associated regular priced paid plans on our [pre-order page](http://flowhub.io/preorder/).

###Kickstarter License
Our [Kickstarter backers](http://noflojs.org/kickstarter/) are welcome to participate in the Flowhub beta testing program. The license rewards from the [Kickstarter](http://www.kickstarter.com/projects/noflo/noflo-development-environment) will be activated in Flowhub at the end of the beta testing period.

###Lifetime Discount
Lifetime discount allows the pre-order license holder to lock-in a discounted rate for future renewals of the associated paid plans. Renewals must be made on a consecutive yearly basis, otherwise the discount will expire. 

###When will the pre-order period end?
As soon as the public release and/or conversion of pre-order licenses into paid plans, expected June 2014.

###What’s the current status of Flowhub?
We are currently in public beta.

###Where is the source code?
Flowhub is built on the [Kickstarter-backed](http://noflojs.org/kickstarter/) open source [NoFlo Development Environment](https://github.com/noflo/noflo-ui), which is available under the MIT license. The productized Flowhub version adds capabilities that require network infrastructure, like GitHub integration, real-time collaboration and runtime discovery.
