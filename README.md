# The Raindance Project

Over the years, we all collect skills in building up attacks and details to help defend and ruggedize our software.  The goal of this project is to figure out how to simplify attack modeling for developers.  And to take on the challenge of making it possible to achieve a good amount of attack modeling within 15 minutes in order to fit within a continuous delivery process.

## Hypothesis

Using github and developing a common components model, we think we can solve for a just enough attack modeling approach that makes it possible to create a better security understanding and strategy for most applications.

## Approach

Raindance builds upon the concept that software projects should contain security information and a common understanding of attack surface.  In a software project that employs this methodology, you would find a SECURITY.md and ATTACKS.md file within the root of the project.  Focusing on the ATTACKS.md file, we believe it is necessary to include a thumbnail sketch along with attacks that have been considered during the design, implementation and operations of the software project.  Further the Raindance Standard is meant to provide a library for commonly implemented patterns and the potential pitfalls that should be considered in order to reduce the effort and time required to identify an attack model.

Systems and services are commonly available from an external, internal, or privileged vantage point.  We have chosen this as the top level entry point to our methodology because it simplifies the initial classification of attack surface.

## Getting Started

### 1. Choose the type of asset you intend to model

Determine if your system will be made available externally, internally, or as a privileged system.  Choose the path that closely aligns with your choice of path to begin your attack model.

If you have multiple classifications, always choose the higher class.  For example, if you have a website that will be used both externally and internally, you will choose the external path to start your model.  Complex attack models will be supported in a later variation of this project.

### 2. Pick a template from the templates library

Right now we have focused on supplying only one template to support basic attack models.

