
#External
![Surface](../../../_images/surface.png) ![External](../../../_images/external.png)

This document contains top-level taxonomy for targets, attacks and mitigations that have been classified as ***external***.  

Choosing an external target in this section means that you have chosen a path that begins with an external target.  This path then gets enumerated by following your target to uncover attacks, weaknesses and mitigations that can be added to your ATTACKS.md file.  You can also arrive at an attack path through one of the other means: Assets, Attacks, or Mitigations.  We'll continue to enumerate and evolve External targets and attack maps in this section.

## External Maps
External maps begin with targets.  Targets are then enriched with attacks and mitigations to help with implementation.  

### Common External Targets

| # | Target| References |Notes|
|---|-------|------------|-----|
|[E0](E0-Organization/README.md)|Organization|R0|Brand, Identity, Reputation, etc.|
|[E1](E1-Physical/README.md)|Physical|R1|Locations, Assets, etc.|
|[E2](E2-Employees/README.md)|Employees|R2|Full-time Employees, Contractors, Partners, etc.|
|[E3](E3-Networks/README.md)|Networks|R3|DMZ, Open Wifi, Public, etc.|
|[E4](E4-Compute/README.md)|Compute|R4|Servers, Proxies, etc.|
|[E5](E5-Products/README.md)|Products|R5|Hard Goods, Services, Software, etc.|
|[E6](E6-Applications/README.md)|Applications|R6|Marketing, Portal, Blog, etc.|
|[E7](E7-Partners/README.md)|Partners|R7|Business, Technology, Support, etc.|
|[E8](E8-Customers/README.md)|Customers|R8|B2C, B2B, etc.|
|[E9](E9-Data/README.md)|Data|R9|Public, Web, Shared, etc.|

### Common External Attacks 

| # |Attack|Common Targets|Potential Mitigations|References|
|---|------|--------------|---------------------|----------|
|[A1](../../../patterns/attack/A1-Unauthorized-Physical-Access.md)|Unauthorized Physical Access|Physical Locations(E1)|Guards(M1), Badges(M2), ||
|A2|Theft|Physical Assets(E1)|Encryption(M3)||
|A3|Reconnaissance|All|||
|A4|Social Engineering|Employees(E2), Partners(E7), Customers(E8)|||
|A5|Denial of Service|Networks(E3), Systems(E4), Web Applications(E6)|||
|A6|||||


### Common Mitigations 

|#|Mitigation|References|Notes|
|---|----------|----------|----|
|M1|Guard Force|||
|M2|Employee Badge|||
|M3|Encryption|||
|M4||||



## Resources

[ISO-27002:8.1]()


