
#External
![External](../../../_images/external.jpg)

This document contains top-level taxonomy for targets, attacks and mitigations that have been classified as ***external***.  We are intentionally reducing complexity in our approach at the top level to make it possible to create attack models in as little as 15 minutes. In other words, we think its important to keep things simple and iterative.

Attack Maps are a work in progress and so its this taxonomy.  We will continue to evolve and grow the framework over time and with contributions.  Our intention is to make use of other existing methods and information available (ex. CAPEC, STRIDE, etc.) to help make this system work for quick attack modeling.

### Common External Targets

| # | Target| References |Notes|
|---|-------|------------|-----|
|[E1](E1-Physical/README.md)|Physical|ISO-27002:8.1|Locations, Assets, etc.|
|[E2](E2-Employees/README.md)|Employees|ISO-27002:8.1|Full-time Employees, Contractors, Partners, etc.|
|[E3](E3-Networks/README.md)|Networks|ISO-27002:8.1|DMZ, Open Wifi, Public, etc.|
|[E4](E4-Systems/README.md)|Systems|ISO-27002:8.1|Servers, Proxies, etc.|
|[E5](E5-Products/README.md)|Products|ISO-27002:8.1|Hard Goods, Services, Software, etc.|
|[E6](E6-Web-Applications/README.md)|Web Applications|ISO-27002:8.1|Marketing, Portal, Blog, etc.|
|[E7](E7-Partners/README.md)|Partners|ISO-27002:8.1|Business, Technology, Support, etc.|
|[E8](E8-Customers/README.md)|Customers|ISO-27002:8.1|B2C, B2B, etc.|
|[E9](E9-Data/README.md)|Data|ISO-27002:8.1|Public, Web, Shared, etc.|

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



