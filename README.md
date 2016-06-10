# The Raindance Project

Over the years, we all collect skills defending our software against attackers and learn the details necessary to make our software more resillient.  The goal of this project is to figure out how to simplify attack modeling for developers by building out component parts and an inheritence model that can be referenced for common attack scenarios and security testing.  Further, we are taking on the challenge of making it possible for a developer to spend 15 minutes developing an attack map that they can keep up to date as their software changes to fit within a continuous delivery process. This will be no small task and we will use what we know already to build out this capability day by day so that we can invite a community of practitioners to help us scale.  We are calling this approach: Attack Maps.

## Hypothesis

Using github and developing a common component model, we think we can solve for a just enough attack mapping to make it possible for developers to get a better sense of how their software will survive in the wild.  The intent of this project is to simplify and focus on how an attacker approaches breaking into software and how it will eventually mesh with Threat Modeling.  

## Approach

The Attack Map approach builds upon the concept that software projects should contain security information and a common understanding of attack surface.  In a software project that employs this methodology, you would find a SECURITY.md and ATTACKS.md file within the root of the project.  Focusing on the ATTACKS.md file, we believe it is necessary to include a thumbnail sketch along with potential attack information considered during the design, implementation and operations of the software project.  Further, this Standard is meant to provide a library for commonly implemented patterns and the potential pitfalls that should be considered in order to reduce the effort and time required to identify an attack model.

We have narrowed our approach for prioritization of common attacks down to three attacker vantage points: external, internal, or privileged.  We have chosen these levels as top level entry points within our methodology because it simplifies the initial classification of attack surface.  Here is a reference diagram to help with understanding how Attack Maps work:

![Top-Level Attack Map](_images/attack-maps.png)

We will begin building out this project using human readable diagrams and dialogue with the intention of automation starting with this top-level depiction.  The intention is to build out a common set of basic building blocks first and then make it possible for more complex scenarios over time.

## Contribute
Raindance is in early stages of being developed by a core team of people who are researching the best ways to accomplish the mission.  We are aware that it looks a bit messy right now as we are assembling the parts and figuring out how to scale our efforts across our community. Raindance can certainly use some additional collaboration.  We're using Slack to start working on this during our free time.  All help is welcome and please realize we are learning how to Open Source, so please be patient with us.

### A. How to help
We are using Omnigraffle and Markdown to start the decomposition of components and to build out the domains. If you want to help there are two avenues:

1. Fork this repo, submit issues and send in pull requests.
2. Reach out to any of the principal contacts on the devsecops.org site.

Work on this project will be slow at first and then it is intended to ramp up over time.  We are also working with some folks that are involved in the [DevSecOps Bootcamp](https://github.com/devsecops/bootcamp)

### B. Where to begin?
We are beginning with External attack surface first and then moving into Internal and Privileged work.  We think this approach will help other folks to adopt sooner and will enable others within the community to assist because of common context.  If you'd like to help us, we think the best place to start is here: [external](external/README.md)

### C. Working with other projects
We are really interested in partnering with other projects that have established common bodies of knowledge.  Our intention is to create a collaborative environment and not a replacement model for other efforts. We have a few open source projects (CAPEC, etc.) identified already and intend to work with them early in this project.


## Getting Started
While we are building out our Attack Map methodology, we would love to gain some early adopters who can help us to understand how to adapt it for wide-scale use.  With this in mind, we have developed a short walkthrough for how to get started:

### 1. Choose an attack path

Determine if your system will be made available externally, internally, or as a privileged system.  Choose the path that closely aligns with your choice of path to begin your attack map.

If you have multiple classifications, always choose the higher class.  For example, if you have a website that will be used both externally and internally, you will choose the external path to start your map.  Complex attack maps will be supported in a later variation of this project.

### 2. Pick a template from the templates library

Right now we have focused on supplying only one template to support basic attack maps.  You can find it in the [templates](templates) directory.

### 3. Set up ATTACKS.md in the root of your project

Describe your project using the template you've chosen and save it as ATTACKS.md in the root of your project.  This file will continue to evolve with your project and when you gain security insights from the instrumentation constructed to support the security feedback loop.

### 4. Link Attack Definitions to ATTACKS.md

Create an /attacks folder in your Test library to have your .attack files run during your build process and/or for run time scans to be kicked off routinely.  Link the .attack to test controls and mitigations routinely.



