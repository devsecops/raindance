# The Raindance Project

Over the years, we all collect skills defending our software against attackers and learn the details necessary to make our software more resillient.  The goal of this project is to figure out how to simplify attack modeling for developers by building out component parts and an inheritence model that can be referenced for common attack scenarios and security testing.  Further, we are taking on the challenge of making it possible for a developer to spend 15 minutes developing an attack map that they can keep up to date as their software changes to fit within a continuous delivery process. This will be no small task and we will use what we know already to build out this capability day by day so that we can invite a community of practitioners to help us scale.  We are calling this approach: ***Attack Maps***. 

This methodology is not a replacement for other security modeling techniques but is necessary for the DevSecOps approach to function well in most organizations.  The intention behind this work is to help value creators to quickly identify blast radius, asset composition, and provide controls for feedback (logging), access control (authentication), and data protection (encryption).

## Hypothesis

Using github and developing a common attack component model, we think we can solve for "just enough" attack mapping to make it possible for developers to get a better sense of how their software will survive in the wild.  The intent of this project is to simplify and focus on how an attacker approaches breaking into software and how it will eventually mesh with Threat Modeling.  

## Approach

The Attack Map approach builds upon the concept that software projects should contain security information and a common understanding of attack surface.  In a software project that employs this methodology, you would find a SECURITY.md and ATTACKS.md file within the root of the project.  Focusing on the ATTACKS.md file, we believe it is necessary to include a thumbnail sketch along with potential attack information considered during the design, implementation and operations of the software project.  Further, this Standard is meant to provide a library for commonly implemented patterns and the potential pitfalls that should be considered in order to reduce the effort and time required to identify an attack model.

We have narrowed our approach for prioritization of common attacks down to three attacker vantage points: external, internal, or privileged.  We have chosen these levels as top level entry points within our methodology because it simplifies the initial classification of attack surface.  Here is a reference diagram to help with understanding how Attack Maps work:

![Top-Level Attack Map](_images/attack-maps-1.png)

We will begin building out this project using human readable diagrams and dialogue with the intention of automation starting with this top-level depiction.  The intention is to build out a common set of basic building blocks first and then make it possible for more complex scenarios over time.

## Catalog
We've organized our work into a living catalog.  Security work generally starts out broad and quickly narrows to become deep and specialized.

* ### [Surface](patterns/surface/README.md)
Attack surface is the entry point for Raindance.  This section describes the top-level for the project and gives you a starting point for your work.   
	
* ### Assets
Assets are the component parts that make up organizations, products, services and other compilations that create value.  Assets are considered property that is owned by an organization or person.

* ### [Attacks](patterns/attack/README.md)
Attacks are steps in an abuse case or exploit or kill-chain that lead to compromise.

* ### Mitigations
Every organization or person has the ability to reduce business risks developed during the value creation process.  Mitigating controls are commonly put in place to make an attack difficult.

##Getting Started
If you want to use this repo to begin establishing your ATTACKS.md file and use the Attack Maps methodology, you can find a starting point here: [GET-STARTED.md](GET-STARTED.md)

##Contributing
If you want to help us with this repo and the Attack Maps work, please read the [CONTRIBUTION.md](CONTRIBUTION.md)


























