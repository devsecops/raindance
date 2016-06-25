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
