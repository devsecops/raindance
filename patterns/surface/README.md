# Surface
![Surface](../../_images/surface.png)

Attack maps often begin with understand the layers of attack surface available to an adversary.  Let's begin with the types of adversaries.  This is not consistent with other methodologies that extend time to threat actors.  We think the threat actor characterizations are important but likely more for security professionals than for value creators.  We'll add some links about threat actors to resources in our [RESOURCES.md](../../RESOURCES.md) over time.

## Lucky or Targeted
The adversary entry point for most attacks is either a lucky find or a targeted attempt. Knowing which of these you are worried about and how is essential in being able to prepare a set of mitigations and appropriate defenses.  A lucky adversary often operates very different from a targeted adversary.  Namely, a lucky adversary tends to find something that was missed or unintended with the goal of understanding where it could lead.  A targeted attacker may have an intended goal and requires a specific set of attacks to be successful to gain access to or information about an intended target.

Some environments make it very difficult to determine whether an adversary is lucky or targeted.  For example, most cloud environments do not provide enough detail to understand whether your asset/target has been identified from a lucky find or targeted reconnaissance.  Similarly, there are combination style attacks that start out lucky with the intention of selling access and entry points to targeted attackers. 

## Enumerating Surface
Enumerating attack surface requires understanding what potential attacks on other resources can do within the trust model that has been established.  Using a simple diagram, you can understand how other resources can be used to further reduce the controls around a specific asset.  Here is a basic enumeration diagram:

![](../../_images/enumeration.png)

In this diagram, the compromise of data, the target, could happen because of a mistake made with the data directly.  It could also happen because of a compromise in another component that shares a trust relationship with data.  Components are generically represented to help the modeler understand when they are asserting trust and how that trust could be used against an asset. This same model is available for all components with complex models able to chain these models together to identify valid attack maps.

Keep in mind that every environment has different and components will be implemented according to business purpose. There are no bullet-proof environments.  We have discovered that keeping attack surface controlled and blast radius contained is often better than attempting to keep attack surface small.  However, the designer is responsible for understanding both considerations, providing rationale and identifying mitigations to support the choice in path.  What works for one environment may not work for others which is why Security is so hard.  

## Surface Entry Points

Using this methodology, attack surface is classified at a top-level as: External, Internal or Privileged.  These entry points provide a vantage point to show the flow and up-leveling of access or attack path: 

* #### [1. External](external/README.md)

	External assets are intentionally or unintentionally exposed for public use or consumption.  Assets that are intentionally exposed publicly are commonly prepared for public access but may not have a full understanding of how they might be abused.  Assets that are unintentionally exposed are commonly not prepared for public access and have attack surface which is more easily abused.

* #### [2. Internal](internal/README.md)

	Internal assets are protected assets that are commonly described under an "ownership" model. Internal assets are not generally exposed to the public and usually include security controls to limit exposure.  Physical and logical boundaries, authentication, and authorization controls are commonly deployed to ensure that only trusted individuals can consume or use these assets.

* #### [3. Privileged](privileged/README.md)
	
	Privileged assets are intentionally well-protected and are certainly not intended for public consumption.  These assets are "handled" by trusted individuals with specified privileges honored by security controls once identification is presented for authorized access to be confirmed.
