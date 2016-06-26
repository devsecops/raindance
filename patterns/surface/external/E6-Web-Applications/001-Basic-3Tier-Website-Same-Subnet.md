# Attack Map: Basic 3-Tier Website / Same Subnet

## Description
An externally available basic website is generally constructed from a core set of components and in many cases is supported by a 2 or 3 tier architecture.  Commonly, a basic website contains a web server, app server and database. In this configuration, the website is configured to share the same subnet with external access through the web server.

## Scope / Dependencies
A typical basic website use case consists of a marketing or blog site with limited to no dependencies.  In this configuration, we are not evaluating the potential for 3rd party integration.

## Diagram  
![E6-001](_images/E6-001.png)        
[![E6-001](../../_images/png-badge.png)](_images/E6-001.png)[![E6-001](../../_images/graffle-badge.png)]()

## Summary Attack Analysis

|#|Attack|Issue/Gap|Reference|Test Reference|Status|
|----|----|----|----|----|----|
|1|Reconnaissance (A3)|Attacker gains information to understand potential weaknesses.|{link to github issue}|{test link}|{workflow status}|
|2|Denial of Service (A5)|Attacker renders website unavailable.|{link to github issue}|{test link}|{workflow status}|
|3|Social Engineering (A4)|Attacker gains customer credentials via social engineering.|{link to github issue}|{test link}|{workflow status}|


## Detailed Attack Analysis

### Attack #1: Reconnaissance
Attackers gain a great deal of insight through reconnaissance activities.

### Attack #2: Denial of Service
Attackers can render websites and web applications unavailable by flooding them with different typs of traffic.

### Attack #3: Social Engineering
Attackers can gain access to authenticated websites and web application by social engineering to obtain credentials directly from unsuspecting customers.

**Notes:**
